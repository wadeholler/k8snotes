## curl to list the databases
curl  http://influx-db-influxdb:8086/query?pretty=true --data-urlencode "q=show databases"
