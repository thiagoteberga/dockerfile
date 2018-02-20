# Docker

#### PostgreSQL 9.3
https://hub.docker.com/r/jetherrodrigues/postgresql/

docker pull jetherrodrigues/postgresql:v1

```sh
sudo docker build -t [your_user_on_docker_hub]/postgresql:[v1] [.]
```

```sh
sudo docker push image:version_tag
```

```sh
sudo docker run -d --name postgresql -p 55432:5432 jetherrodrigues/postgresql:v1
```

```sh
sudo docker stats postgresql
```

```sh
sudo docker port postgresql
```
Connect to docker postgresql (user: docker, password: docker)
```sh
psql -h localhost -p 55432 -d docker -U docker --password

docker=# select datname from pg_database;
docker=# create database unisal;
```

#### JAVA 8
docker pull jetherrodrigues/my_java:v1

Compile the java file
```sh
sudo docker run --rm -v $PWD:/[app path] -w /[app path] jetherrodrigues/my_java:v1 javac Main.java
```
Execute the bytecode(.class) file
```sh
sudo docker run --rm -v  $PWD:/[app path] -w /[app path] jetherrodrigues/my_java:v1 java Main
```

#### Maven


#### Application
