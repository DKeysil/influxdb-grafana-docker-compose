# InfluxDB + Grafana + docker-compose
---
Clone this repo
```
git clone https://github.com/DKeysil/influxdb-grafana-docker-compose.git
```

Change users and passwords in `docker-compose.yml` if you want

Make two dirs
```
mkdir {grafana-data,influxdb}
```

Run it
```
docker-compose up -d
```

Then you'll have access to Grafana from browser by `http://localhost:3000`
Open it, login in and then add `Data source`:
1. Choose InfluxDB
2. In HTTP set url `http://influxdb:8086`
3. In InfluxDB Details set Database name, user and password
4. If after clicking "Save and test" you have green alert - everything is fine

## That's all
