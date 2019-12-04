# Angular-RDB
Access to RDB from Angular using @ngrx/data and ActiveRecord

## Preparation
1. git clone this repository in your local disk
2. cd Angular-RDB
3. docker-compose build
4. docker-compose up
5. docker-compose down   close and delete images

*2 docker containers (activerecord-service & database) UP

## Running
1. If you want run compiled Angular then input following in your browser.
    http://localhost:4567/

2. If you want see source and implement do following .
   ng new newproject
   cd newproject
   ng add @ngrx/store
   ng add @ngrx/effects
   ng add @ngrx/entity
   ng add @ngrx/data
   ng add @angular/material
   npm i @angular/flex-layout --save

   remove src directory
   copy src directory from repository

   edit angular.json following
          :
          :
    "serve": {
    "builder": "@angular-devkit/build-angular:dev-server",
    "options": {
    "browserTarget": "ngrxdata-activerecord:build",
    "proxyConfig": "src/proxy.conf.js"  <- add this line for api cross
    },

## Version
Angular  8.2.14 need > 8.x.x
ngrx  8.5.2  need > 8.x.x
MySQL 5.7
Ruby 2.6.5
sinatra
