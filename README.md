# mosquitto-broker

To get temperature readings only:

```
docker-compose exec broker mosquitto_sub -v -t '/+/temp'
```

To get everything: 

```
docker-compose exec broker mosquitto_sub -v -t '#'
```

To get moisture readings (or other ADC):

```
docker-compose exec broker mosquitto_sub -v -t '/+/io2'
```

