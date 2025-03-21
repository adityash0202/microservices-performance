# DCS_PROJECT
# django-microservices
Django Microservices Project using Docker, nginx and Django REST Framework

Overview
--------
We have 3 docker containers:

* polls: runs the polls service
* questions: runs the questions service
* votes: runs the votes service

Requirements
------------
* docker
* docker-compose

Usage
-----

    $ docker-compose up

Deployment Requirements:
We have used PostgreSQl. In serverless GCP was connected to our database but its credentials are valid for only 7 days. After every 7 days user needs to use new credentials, so please create new one if it seems expired.
For serverful deployment please create new Google compute engine instance which is required for this serverful deployment, because our instance can be used only by our own GCP credentials. 
All other requirements and dependecies are present in our microservices.


