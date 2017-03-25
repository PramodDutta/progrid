![alt text](https://d30y9cdsu7xlg0.cloudfront.net/png/2143-200.png "ProdGrid")

# ProGrid v1.0
Run Selenium hub with VNC supported Firefox and Chrome  with scale feature with the simple compose commands.

Welcome to the ProGrid:
Author : Pramod

By Default up and Scale to 3FF and 1Chrome
```
$ docker-compose up -d
$ docker-compose scale nodechrome=1 nodefirefox=3
```
Down the Grid

```
$ docker-compose down
```
Start the Grid
```
$ docker-compose start
```
Stop the Grid
```
$ docker-compose stop
```

Restart with new Node
```
$ docker-compose scale nodechrome=0 nodefirefox=4
$ docker restart progrid
```
### GRID running at 
```
127.0.0.1:4444/grid/console
```

#### Attach to VNC ,

To see the VNC port run 
```
$ docker-compose ps
```
You will see something like this
0.0.0.0:32798->5901/tcp ( Open SAFARI and vnc://0.0.0.0:32798 )
> VNC password is 'secret'.


# Todo !

  - Videos Support & Dashboard
  - Run Code directly from the Jenkins(Jenkins will create a docker container and Run and  stop it after.

License
----

MIT

