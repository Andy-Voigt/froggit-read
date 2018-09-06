# froggit-read
Readout Froggit FT007PF temperature sensors

Simple readout helper based on [adilosa/weathermon](https://github.com/adilosa/weathermon) github project to debug my Froggit FT007PF pool thermometer sensor.

create a sqlite3 db under /opt/weather.db

```
sqlite3 weather.db
sqlite> create table reading(id INTEGER PRIMARY KEY, channel INTEGER, temperature REAL, humidity INTEGER, battery INTEGER,  date TIMESTAMP DEFAULT CURRENT_TIMESTAMP);
sqlite> .exit
```
