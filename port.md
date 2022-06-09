# Port Learn

## install lsof
```shell
$ sudo yum -y install lsof
```

## check all listening port
```shell
$ sudo lsof -i -P -n | grep LISTEN
```

## check one listening port
```shell
$ sudo lsof -i -P -n | grep :80
or
$ sudo lsof -i:8080
```

## to kill any process listening port 
```shell
$ sudo kill $(lsof -t -i:80)
or more violently
$ sudo kill -9 $(lsof -t -i:80)
```