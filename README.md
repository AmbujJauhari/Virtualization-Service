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
5. Mappings can be shared to public -> public mappings can only be edited by raising a pull request and this has to be approved by the owner of the mappings
7. Integration in the environment
8. Can act as a proxy
9. SSO implemented via github
10. Custom module to handle configurations because to be able to deployable we need to be able to perform customization like SSO via github or SSO via gitlab or SSO via custom LDAP networks. This is also extendable to use custom tools like someone might be using gitlab pipeline and not the azure devops pipeline. So we need the core microservices to be free from this dependencies instead these dependencies need to be handled by separate individual services. one for devops, one for SSO

# Distribution
Deployment and distribution happens using helm chart

# Possible list of microservices

1. HTTP
2. RMI
3. IBM
4. Tibco
5. JMS
6. Kafka
7. Mappings
8. Auth
9. Devops (might be a utility) -> Question will be like how will be make sure the code for devops sits close to each module but also how to separate out the concern for having different tools.
10. 

# Deployment
1. Local deployment happens using helm chart on minikube
2. Azure deployment happens using terraform and AzureDevOps pipeline or custom pipeline
