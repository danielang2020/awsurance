# awsurance
An insurance application based on AWS and K8s. want to experiment with cloud native.


## 1. Product Facility Domain
1.1 product crud \
1.2 calculate according to product spec. including premium, face amount, and death benefit.

## 2. new business service domain
1.1 create a new policy \
1.2 because the fields of a policy will be added in the future, so will use dynamodb to store proposal information.
   
## 3. Underwriting service domain
2.1 if creating(before inforce) or updating(after inforce) a policy will be validated on some rule, check it manually or according to a pre-defined rule, could be approved automatically.
   
## 4. policy/customer service domain
3.1 Customers want to update policy information, sometimes update automatically and sometimes need to underwrite to update.
   
## 5. claim service domain
4.1 When a claim(a special cs) is requested, the latest policy information must be retrieved as evidence, and then disbursement must be handled based on the evidence.
   
## 6. User/agent service domain
7.1 manage user and agent information, the user is a system user who can log in to the system to handle biz, and likewise, an agent is a sales agent who can sell policies to customers.

## 7. arap service domain
8.1 receive premium, pay disbursement/death benefit, etc.
   
## 8. rule service domain(external)
9.1 some rules need to be set in advance, when a new policy or some other thing that needs to update policy, will be checked by it.
   
## 9. workflow service domain
10.1 the insurance company has different positions that only handle their biz, automatically assign tasks to the right one.

## 10. analysis
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
