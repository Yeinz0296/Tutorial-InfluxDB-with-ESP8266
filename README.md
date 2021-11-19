# Tutorial-InfluxDB-with-ESP8266

## Intalling InfluxDB

### System requirements:
- Windows 10
- 64-bit AMD architecture
- Powershell or Windows Subsystem for Linux (WSL)

### Command line examples
Use Powershell or WSL to execute `influx` and `influxd` commands. The command line examples in this documentation use `influx` and `influxd` as if installed on the system PATH. If these binaries are not installed on your PATH, replace `influx` and `influxd` in the provided examples with `./influx` and `./influxd` respectively.

1. [Download the InfluxDB](https://docs.influxdata.com/influxdb/v2.1/install/?t=Windows)
2. Extract the zip file into C:\Program Files\InfluxData
3. Open CMD and input the command
```cmd
cd \Program Files\InfluxData & influx
```
4. When run for the first time, Windows Defender will appear with the following message:
> Windows Defender Firewall has blocked some features of this app.
5. Click Allow access

## Set up InfluxDB through the UI
1. By default the TCP Port is `8086`
2. The InfluxDB can be access by accessing `localhost:8086` or `http://Your_Local_IPADRRESS:8086`

## Set up your initial user
1. Enter a Username for your initial user.
2. Enter a Password and Confirm Password for your user.
3. Enter your initial Organization Name.
4. Enter your initial Bucket Name.
5. Click Continue.

InfluxDB is now initialized with a primary user, organization, and bucket. You are ready to write or collect data
