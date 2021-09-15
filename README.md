# sonarqube-deploy

## This Docker Compose YAML run two services:
 - db
 - sonarqube

### System requirements:
 - sysctl -w vm.max_map_count=524288
 - sysctl -w fs.file-max=131072
 - ulimit -n 131072
 - ulimit -u 8192
 - expose port 9000

### to start:
 - sudo docker-compose up -d

### to stop:
 - docker-compose stop

### to destroy and erase volumes:
 - docker-compose down --volumes