# strapi-dockerization

## Create Strapi project

If you running this for the first time then you need to comment and uncomment below lines in the docker-compose.yaml file.
- Comment line 17.
- Uncomment line 16.

## Running an existing Strapi project

Once the project is created we can directly run the project as the volumes are mapped. For this make the below changes to the docker-compose.yaml file.
- Comment line 16.
- Uncomment line 17.

## Dockerfile.createproject

This file is written to create a strapi project at /srv/app location in the container.

## Dockerfile.runproject

This file is written to run the existing strapi project. The volumes are mapped so there will be 2 folders in local that are mapped to the container
- strapi: This folder holds the Strapi project frontend.
- strapi-db: This folder holds the postgres database of the strapi app.
