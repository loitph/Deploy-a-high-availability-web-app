# Deploy a high-availability web app using CloudFormation
This is one of the project in Udacity Cloud DevOps Engineer Nanodegree.

## Project Overview
Assume that one company is creating Instagram like application. Developers have developed the code and pushed the code into the S3 bucket on AWS. Now the task is to create the infrastructure for deploying that application in an automated way using CloudFormation following the best practices and once infrastructure is ready, deploy that application code onto that high availability infrastructure.

## Project Files

- `network.json`: Parameter file for Network CloudFormation.
- `network.yaml`: Template file for Network CloudFormation.
- `server.json`: Parameter file for Server CloudFormation.
- `server.json`: Template file for Server CloudFormation.

## Project Setup

- Create Network:
  + Template:
  ```
  ./create.sh <<stack name>> <<template file>> <<parameter file>>
  ```
  + Sample usage:
  ```
  ./create.sh loitph-network-stack network.yaml network.json
  ```

- Create Server:
  + Template:
  ```
  ./create.sh <<stack name>> <<template file>> <<parameter file>>
  ```
  + Sample usage:
  ```
  ./create.sh loitph-server-stack server.yaml server.json
  ```