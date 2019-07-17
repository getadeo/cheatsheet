# Start
```
$ docker-compose up
```

# Start (usind a json config)
```
$ docker-compose -f docker-compose.json up
```

# Start in background
```
$ docker-compose up -d
```

# Stop
```
$ docker-compose down
```

# Start 8 instances of app
```
$ docker-compose up --scale <service_name>=8
```

# Start 8 instances of app in background
```
$ docker-compose up --scale <service_name>=8
```