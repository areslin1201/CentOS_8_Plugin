# Nginx
> Nginx version [link](https://nginx.org/)


## 1.check Nginx default version in Centos
```shell
$ sudo yum module list nginx
```

```shell
CentOS Stream 8 - AppStream
Name                  Stream                   Profiles                  Summary                       
nginx                 1.14 [d]                 common [d]                nginx webserver               
nginx                 1.16                     common [d]                nginx webserver               
nginx                 1.18                     common [d]                nginx webserver               
nginx                 1.20                     common [d]                nginx webserver               

Hint: [d]efault, [e]nabled, [x]disabled, [i]nstalled
```
you can get this,and the default version is 1.14


## 2.choose other version
```shell
$ sudo yum module reset nginx
$ sudo yum module enable nginx:1.20
$ sudo yum module list nginx
```


## 3.install nginx
```shell
$ sudo yum -y install nginx
```


## 4.check nginx version
```shell
$ nginx -v
```


## 5.enable nginx server
enable nginx service so that it start at server boot time
```shell
$ sudo systemctl enable nginx
```


## 6.start the service
```shell
$ sudo systemctl start nginx
```


## 7.other we need commands
```shell
$ sudo systemctl start nginx
$ sudo systemctl stop nginx
$ sudo systemctl restart nginx
$ sudo systemctl reload nginx
$ sudo systemctl status nginx
```