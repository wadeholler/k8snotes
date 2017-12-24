## curl to list the databases

    curl  http://influx-db-influxdb:8086/query?pretty=true --data-urlencode "q=show databases"

## create a database

    curl -XPOST -G http://influx-db-influxdb:8086/query --data-urlencode "q=CREATE DATABASE mydb"
