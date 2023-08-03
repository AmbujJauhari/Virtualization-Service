# Virtualization-Service

A single application built of multiple microservices communicating together. It will be built on the concept that each team is responsible for their own product components what that means is each team works vertically owning their own microfront end, the logical business layer and the database of their own choosing. 

Protocols supported

1. HTTP / HTTPs
2. RMI
3. JMS
4. IBM MQ
5. Tibco
6. Kafka


# Front end
Front end will be composed of multiple microfront ends written in dart

# Back end
Back end components are written in python

# Database
Mongo Db is the choosen DB to store the mappings

# Features
1. Recording
2. Integration options with CI / CD pipeline
3. Run on local only pre-requisite is to have docker
4. Each user get their own profile page to CRUD the mappings
5. Mappings can be shared to public
6. Integration in the environment
7. Can act as a proxy

# Distribution
Deployment and distribution happens using helm chart

# Deployment
1. Local deployment happens using helm chart on minikube
2. Azure deployment happens using terraform and AzureDevOps pipeline or custom pipeline
