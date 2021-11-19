# Explaination

```ino
#if defined(ESP32)
#include <WiFiMulti.h>
WiFiMulti wifiMulti;
#define DEVICE "ESP32"
#elif defined(ESP8266)
#include <ESP8266WiFiMulti.h>
ESP8266WiFiMulti wifiMulti;
#define DEVICE "ESP8266"
#endif
```
This will check either you are using `ESP32` or `ESP8266`

```ino
#include <InfluxDbClient.h>
#include <SimpleDHT.h>
int pinDHT11 = D1;
SimpleDHT11 dht11(pinDHT11);
```
We will be using 2 Libraries in this sample coding. [InfluxDBClient by Tobias](https://github.com/tobiasschuerg/InfluxDB-Client-for-Arduino) and [SimpleDHT by Winlin](https://github.com/winlinvip/SimpleDHT)
> Both can be download using Arduino IDE libraries manager

```ino
// WiFi AP SSID
#define WIFI_SSID "ssid"
// WiFi password
#define WIFI_PASSWORD "password"
// InfluxDB  server url. Don't use localhost, always server name or ip address.
// E.g. http://192.168.1.48:8086 (In InfluxDB 2 UI -> Load Data -> Client Libraries), 
#define INFLUXDB_URL "influxdb-url"
// InfluxDB 2 server or cloud API authentication token (Use: InfluxDB UI -> Load Data -> Tokens -> <select token>)
#define INFLUXDB_TOKEN "toked-id"
// InfluxDB 2 organization id (Use: InfluxDB UI -> Settings -> Profile -> <name under tile> )
#define INFLUXDB_ORG "org"
// InfluxDB 2 bucket name (Use: InfluxDB UI -> Load Data -> Buckets)
#define INFLUXDB_BUCKET "bucket"
// InfluxDB v1 database name 
//#define INFLUXDB_DB_NAME "database"
```
