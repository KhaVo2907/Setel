# In this project, we’ll build a NodeJS microservice and deploy it using a Docker Swarm Cluster.
# The tools we're going to use:
    NodeJS version 10.15.3
    MongoDB 4.0.6
    Docker 
# Architecture for microservice
    UI <----> (Rest API) Order Service <-----> (Rest API) Payment Service
                    |
                    |
                 MongoDB
## This is structure of project:
    Setel
    ├── docker-compose.override.yml
    ├── docker-compose.yml
    ├── README.md
    └── src
        ├── order-application       # Order service build on loopback framework
        │   ├── common
        │   ├── Dockerfile
        │   ├── package-lock.json
        │   ├── package.json
        │   ├── README.md
        │   └── server
        ├── order-frontend          # UI application using to take order by user. Build on ReactJS libraries
        │   ├── config
        │   ├── Dockerfile
        │   ├── package-lock.json
        │   ├── package.json
        │   ├── public
        │   ├── README.md
        │   ├── scripts
        │   └── src
        └── payment-application     # Payment service built on ExpressJS, TypeScript, Webpack
            ├── dist
            ├── Dockerfile
            ├── package-lock.json
            ├── package.json
            ├── src
            ├── tsconfig.json
            ├── tslint.json
            ├── webpack.config.js
            └── webpack.config.prod.js

# Prerequisite
    - Docker
# Run
    - docker-compose up
