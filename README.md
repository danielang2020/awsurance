# awsurance
An insurance application based on AWS and K8s. want to experiment with cloud native.


## 1. Elastic Product Facility Domain, including calculation
1.1 product crud \
1.2 provide product mandatory info and related formula and rate table. \
1.3 product info should be version-controlled. \
1.4 elastic product management

## 2. Policy Management Domain
1.1 store inforce policy \
1.2 maintain policy model and make it cohesion \
1.3 calculate based on product info. \
1.4 store every version once update is done.(Copy and write) \
1.5 elastic policy management \
1.6 seperate cud and r, coz when run day end batch, cud are not allowed.

## 3. Policy Workflow
1.1 NB/UW/Claim workflow process \
1.2 Claims only refer to the specific policy version when the claim happens. \
      
## 4. User/agent service domain
7.1 manage user and agent information, the user is a system user who can log in to the system to handle biz, and likewise, an agent is a sales agent who can sell policies to customers.

## 5. arap service domain
8.1 receive premium, pay disbursement/death benefit, etc.
   
## 6. rule service domain(external)
9.1 oauth2/saml \
9.2 activity(bonus)

## 7. analysis
11.1 according to the biz data, some trends will be analyzed and some reports will also be generated. \
11.2 column db will be used. such as redshift.

## 8. day end batch
8.1 a job could be executed by batch trigger or real time trigger. 

eks + spot instance/fargate \
cognito \
keda for pod, carpenter for node \
springboot/quarkus/grpc/fastapi \
opentelemetry \
telepresence  \ 
spring-boot-data-source-decorator/flexy pool \
Terraform \
Spring Cloud Kubernetes Watcher for automatically reload configuration \
rds with secret manager automatically rotation \
HikariCP \
Chaos Mesh \
R2DBC \
AWS Batch + Step Functions + eks for workflow \
python + LaTeX(SymPy) + mathJax (sympy Piecewise could express if logic) \
query product or policy info using graphql \

k8s: crossplane, argocd, opentelemetry(prometheus/grafana)
