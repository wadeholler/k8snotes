## running influx-db with helm example

helm install --name influx-db --set persistence.enabled=true,persistence.storageClass=gp2,service.type=LoadBalancer   stable/influxdb
