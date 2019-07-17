# Run File
```
$ docker run --rm -v $(pwd):/src python:3 python /src/hello.py
```

# Run interpreter
```
$ docker run --rm -it -v $(pwd):/src python:3 python
```

# Open a shell in the container
```
$ docker run --rm -it -v $(pwd):/src python:3 /bin/bash
```

# Build custom image
```
$ docker build -t python_numpy .
```

# Run file
```
$ docker run --rm -v $(pwd):/src python_numpy python /src/hello.py
```

# Open a shell in the container
```
$ docker run --rm -it -v #(pwd):/src python_numpy /bin/bash
```

# Start container in foreground
```
$ docker run --rm -v $(pwd):/usr/share/nginx/html -p 8080:80 nginx:latest
```

# Start container in background
```
$ docker run --rm -d -v $(pwd):/usr/share/nginx/html -p 8080:80 nginx:latest
```

# open a shell in the container
```
$ docker run --rm -it -v $(pwd):/usr/share/nginx/html nginx:latest /bin/bash
```

# See running containers
```
$ docker ps
$ docker container ls
```

# Logging in to running container
```
$ docker exec -it <container_name   > /bin/bash
```

# Create a network to allow sharing between containers
```
$ docker network create <network_name>
```

# Create mysql container
```
$ docker run --rm -d --net <network_name> --name mul_mysql -e MYSQL_ROOT_PASSWORD='root' mysql:5.6
```

# Create (and open a terminal into) node.js container
```
$ docker run --rm -it --net <network_name> --name mul_node node:8 /bin/bash
```




