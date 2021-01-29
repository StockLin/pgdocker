# Instructions
## Create presist volume
-   ``` 
    docker volume create pgdata
    ```

## Run the composer
-   ``` 
    docker-compose up -d
     ```

## Explaination
- when container up, postgreql image will create default
    - superuser: postgresql
    - db: postgresql
    - password: config from  environment variable（POSTGRES_PASSWORD） settings
- Extras
    - Changing environment variable POSTGRES_USER & POSTGRES_DB from compose yml to change the default dbname and superuser name


##### References
-   [DockerHub postgresql](https://hub.docker.com/_/postgres/) 