## Docker Engine setup on MAC

### Install Docker & docker compose cli

```Bash
brew install docker
brew install docker-compose
```

Verify that the docker cli is working
```Bash
docker --version
```

### Install Colima & Start docker server

```Bash
brew install colima
```

Start Colima
```Bash
colima start
```
or if you are using an M1 machine, you can use the following command:
```Bash
colima start --profile amd --arch amd
```

Verify that the docker client & server are working
```Bash
docker ps
```

You should see the following output at this point if your installation was correct
```
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
```

### Kill the docker engine
```Bash
colima stop
```










