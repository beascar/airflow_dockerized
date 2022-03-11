# KRI65 - Airflow_2_2
This project helps to setup KRI65 with airflow 2.2 in Docker.


## General Usage Notes:

### Before cloning this repo:

* Install Docker on your machine.
* Setup enough memory under Docker setting section as shown below:
    - Follow confluence link https://manulife-ets.atlassian.net/wiki/spaces/CSEA/pages/12365660325/Running+Airflow-2.2+in+Docker for more illustrations.
* Install git on your machine.


### After cloning this repo:
* Run docker file by using command: `docker-compose up airflow-init `
* Once the previous command completes, run `docker-compose up`
* To verify local airflow instance, in browser try http://localhost:8080/home.  
    - If prompted, use the following credentials:

    Username: airflow

    Password: airflow

* Stop services:
    - if we want bring down and clean up all the containers then run command: `docker-compose down`

* Rename docker-compose.yaml to docker-compose.yaml.init
* Rename docker-compose.yaml.flyway to docker-compose.yaml
* Run command `docker-compose up`
* Then follow the instruction in the "Flyway migrations" section of (this confluence document)[https://manulife-ets.atlassian.net/wiki/spaces/CSEA/pages/12365660325/Running+Airflow-2.2+in+Docker#Step-3.--Flyway-migration%3A]

