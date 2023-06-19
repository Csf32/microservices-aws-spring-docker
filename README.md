# Microservices-AWS-Docker-Spring

# 1. How to Create and Running app in a Docker Container
  
  1.1 Install grandle build in vscode: <br>
  >Configure Dockerfile before create build <br>
  >Open the terminal put the code to create build folder: **./gradlew build**

  1.2 Create docker image: <br>
  
  >Paste in terminal: **docker build -t <Name of your image (name of baseName on bootJar)>:1.0.0 .**
  
  1.3 Create docker container: <br>
  >Paste in terminal: **docker run -p <Your host, for exemple: 8080:8080> <Name of your image (name of baseName on bootJar)>:1.0.0** <br><br>

  1.4 Push to docker hub:
  >Paste in terminal while running in your host: **docker push your username/name of image:version** <br><br>
  

# 2.Run VPC - AwsCdkProject
 
2.1 Install AWS CLI <br> 

2.1.1 Install apps 
>Firrtly, you need to install Java JDK 15+, Apache 3.5+ and Node.JS 10+ <br> 

2.1.2 Install AWS CLI from AWS website
>**https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html**  <br> 

2.1.3 Configure AWS IAM Account 
>In your Users in AWS IAM account, add user with access key ID and secret access key<br> <br>

2.1.4 Configure Your Credentials CLI In Terminal 
>Open the terminal of OS and your path of CLI and configure with your credentials using: **./aws configure**<br><br>

2.2 Install AWS CDK <br>

2.2.1 Configure AWS CDK: <br>
>Open the terminal of OS and install globally: **npm install -g aws-cdk** <br>

2.2.2 Create Project CDK: <br>
>Create a folder of your CDK project and past of path terminal: **cdk init app --language java** <br><br>

2.3 Create VPC 
>cdk bootstrap
>Create Stack Vpc: **cdk deploy Vpc**

