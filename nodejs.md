# NodeJS
> NodeJS version [link](https://nodejs.org/en/download/)


## 1.check NodeJS default version in Centos
```shell
$ sudo yum module list nodejs
```

```shell
CentOS Stream 8 - AppStream
Name            Stream         Profiles                                      Summary                   
nodejs          10 [d]         common [d], development, minimal, s2i         Javascript runtime        
nodejs          12             common [d], development, minimal, s2i         Javascript runtime        
nodejs          14             common [d], development, minimal, s2i         Javascript runtime        
nodejs          16             common [d], development, minimal, s2i         Javascript runtime        

Hint: [d]efault, [e]nabled, [x]disabled, [i]nstalled
```
you can get this,and the default version is 10


## 2.choose other version
```shell
$ sudo yum module reset nodejs
$ sudo yum module enable nodejs:16
$ sudo yum module list nodejs
```


## 3.install NodeJS
```shell
$ sudo yum -y install nodejs
```


## 4.check NodeJS/npm/npx version
```shell
$ node -v
$ npm -v
$ npx -v
```