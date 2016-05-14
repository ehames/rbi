# rbi
Replicable Build Infrastructure - quickly setup a complete CI/CD infrastructure for your project

## Experimental CI
Run the experimental CI services using docker-compose.

### Run
```bash
$ docker-compose -f docker-compose-drone.yml up
```
### Configure
1. Find your docker-host ip address and set it the REMOTE_CONFIG variable of drone in the docker-compose-drone.yml
1. Configure the Gogs service: Open your browser and point http://docker-host:3000
1. Login to Drone CI using the credentials created in step above http://docker-host

### TODO
- store build metrics in Sonar (?)
- set up code review service
