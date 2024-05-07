# Sonarcube docker compose
Here is a container version of docker compose to deploy it you must have the following

1. Docker already installed
2. At least 2GB of RAM with at least 1GB of free RAM
3. 10 GB of free space

once the condition are met the next step is to configure vm.max_map_count to do so if 

For MS Windows users, using wsl subsystem Open powershell, run
```
$wsl -d docker-desktop
```
then 
```
sysctl -w vm.max_map_count=262144
```
For linux users
```
sysctl -w vm.max_map_count=262144
```

Clone the repository
```
git clone https://github.com/YeKoEliteMLOPS/sonarqube.git
```
then
```
cd sonarqube
```

then run docker compose command

```
docker compose up -d
```

To open it, go to localhost:9000 and the username and password are both admin
