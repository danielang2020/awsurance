# awsurance
An insurance application based on AWS


## 1. Product Facility
1.1 product crud \
1.2 calculate according to product spec.





## 1. new business service domain
1.1 create a new policy \
1.2 because the fields of a policy will be added in the future, so will use dynamodb to store proposal information.
   
## 2. Underwriting service domain
2.1 if creating or updating a policy validates some rule, check it manually.
   
## 3. customer service domain
3.1 Customers want to update policy information, sometimes update automatically, and sometimes need to underwrite to update.
   
## 4. claim service domain
4.1 When a claim is requested, the latest policy information must be retrieved as evidence, and then reimbursement must be handled based on the evidence.
 
## 5. policy service domain
5.1 store all policy information whose status is in force. \
5.2 The history of policy change and maintenance of policy versions need to be stored. 
   
## 7. product service(calculate) domain
6.1 provide product detail information including premium formula etc.
   
## 8. User/agent service domain
7.1 manage user and agent information, the user is a system user who can log in to the system to handle biz, and likewise agent is a sales agent who can sell policies to customers.

## 9. arap service domain
8.1 receive premium, pay reimbursement.
   
## 10. rule service domain(external)
9.1 some rules need to be set in advance, when a new policy or some other thing that needs to update policy, will be checked by it.
   
## 10. workflow service domain
10.1 the insurance company has different positions that only handle their biz, automatically assign task to right one.

## 11. analysis
11.1 according to the biz data, some trends will be analyzed and some reports will also be generated. \
11.2 column db will be used. such as redshift.


eks + fargate \
cognito \
keda \
springboot/quarkus/grpc \
opentelemetry \
telepresence  \ 
spring-boot-data-source-decorator/flexy pool \
Terraform \
Spring Cloud Kubernetes Watcher for automatically reload configuration \
rds with secret manager automatically rotation \
HikariCP \
Chaos Mesh 
