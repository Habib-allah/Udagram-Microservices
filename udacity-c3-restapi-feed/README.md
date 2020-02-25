# Udagram Image Filtering Microservice

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

The project is split into three parts:
1. [The Simple Frontend](https://github.com/grutt/udacity-c2-frontend)
A basic Ionic client web application which consumes the RestAPI Backend. 
2. [The RestAPI Backend](https://github.com/grutt/udacity-c2-restapi), a Node-Express server which can be deployed to a cloud service.
3. [The Image Filtering Microservice](https://github.com/grutt/udacity-c2-image-filter), the final project for the course. It is a Node-Express application which runs a simple Python script to process images.

## UPDATE (VERY IMPORTANT):
I wrapped getGetSignedUrl getPutSignedUrl in Promises in order to fix asynchronous credential fetching with Typescript/Javascript, otherwise you won't get a valid url to access the S3 Bucket. (./src/aws.ts) 

