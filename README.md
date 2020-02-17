# DHIS2 with Docker

# Running

To start DHIS 2 and Postgres database

```
docker-compose up -d
```

To shut down DHIS 2 and Postgres database

```
docker-compose down
```

## DHIS2 with pre-populated Postgres database using Docker Compose

Steps:

- Create the SQL file with the schema and data you want for pre-populate Postgres with into the `config/` directory. For example, you can download a [sample DHIS 2 database](https://www.dhis2.org/downloads), and extract the sql file in the archive.
- (Re)name the file to `init-db.sql`.
- Use the command below to start up your containers:

    ```
    docker-compose -f docker-compose-with-populated-db.yml up -d
    ```

More detailed notes about seeting up DHIS2 with Docker is available [here](https://developers.dhis2.org/2019/10/dhis2-and-docker/).