# Airflow_2_2
This project helps to setup airflow 2.2 in Docker.


## General Usage Notes:

### Before cloning this repo:

* Install Docker on your machine.
* Setup enough memory under Docker settings
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


