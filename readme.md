Make sure you have a local docker instance of rabbit mq running

First install composer dependencies
```bash
./init.sh
```

Then start the rabbitmq container and the app
```bash
docker-compose up
```

You can now go to localhost:8080 and watch your events be generated when you send them to the rabbitmq server

# One

Go to the first example
```bash
cd one
```

First be ready to receive commands
```bash
./receive.sh
```

Then send a command
```bash
./send.sh
```

You should now see the receive.sh script echo:
```
[x] Received Hello World!
```
