# Project- Full Stack and Deployment on AWS CircleCi Github....

#### Apllication Infrastructure

#### First We got the Technologies:

- AWS (Amazon Web Services) :

1- RDS (Relational Database):

- We create database based on our need , Capacity ,Scalability, Encryption , Backup and so on.
- Here is my LOCALHOST: database-1.coek0br4cgsf.us-east-1.rds.amazonaws.com
- Although this is public database.

2- S3 (Bucket)

- This is the store of our Frontend app also after marking it as static web site we got the link.
- Here is my link: http://udagram-hassan.s3-website-us-east-1.amazonaws.com/

3- EB (Elasticbeanstalk)

- this is the store of our backend app although it has a link to check the routs and the data if we want.
- Here is my link: http://udagram-env.eba-papka3yu.us-east-1.elasticbeanstalk.com/

-CircleCi (CI/CD framework)

- We use this framework to make a continous Integgeration

- Also we can offer Continuous Deployments

................................................................................................................................

### 1- First In this project this some of the used modules in the project:

##### 1-Node Package Manager v[14.15.0]

##### 2-Bestzip package v[2.2.1]

##### 3-Typescript v[3.9.10]

##### 4-Postgres pg v[8.7.1]

##### 5-AWS CLI v[2.7.16]

##### 6-EA CLI (Elasticbeanstalk) v[3.20.3]


................................................................................................................................

## Pipeline Process

## First of all everyone has his own way to achieve and this is my own idea:

#### 1- Creating the Database in AWS RDS and store the parameter in .env file.

#### 2- Link the local application to Github Through pushing it.

#### 3- Link the CircleCLI Directly to Github throught signing in and link Github.

#### 4- After That Pass all the enviromet variable to the enviorment variable CircleCi and create the circlecli in the main directory of the full project.

#### 5- If the repo has been changed then Circlecli starts the CI then deployment to AWS.

#### 6- Through First Installing all the dependencies that's need to deploy the application in both front and back end seperately.

#### 6- After that in our application the deployment related to the manager to approve it.

#### 7- When the manager approve it Starting the deployment of front end in the S3 Bucket.

#### -8 IF the previous is successful then deployment of the backend will take place.

#### 7- IF there is any error in Pipeline in CircleCi the process stoped and also the deployment will not happen.


### Mohamed Hassan Project  Application Development and Deployment