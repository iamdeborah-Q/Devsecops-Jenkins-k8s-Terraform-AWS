
# IMPLEMENTATION OF OF DEVSECOPS WITH JENKINS-TERRAFORM-AWS INFRA

Devops has made it possible to develop application in a fast quicker time by time by aligning development, test and production tea, however in most most cases security is not intergrated in the development process and test becomes vulnerable to risks of bugs. Here is where DevSecOps comes into the picture. The DevSecOps approach includes incorporating security as significant components of DevOps practices. Whiles DevOps refers to collaborating of developments, testing of operation team to achieve continues delivery, DevSecOps involves the intergration of security with the sane DevOps process. Devops includes several areas of focuse which inclufdes Automated provisioning, continues Monitoring, continues intergration and test driven developments. As an extension of DevOps Midset, DevSecOps is the methodology of intergrating security tools i into the devOps process.
In this Projects an EasyBuggie Vulnerability web Application was develops using Terraform, Kubernetes and AWS


The Diagram belows show th steps used to implement this project

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/36695ba8-8970-4a5e-82b1-1609c1a614fd)


DevSecOps Tools 

                  SCA scan -
                  SAST scan -
                  DAST scan -




STEP: 1. Create AWS Admin User and Install AWS CLI nad Authenticate with AWS

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/202415f1-73d3-47c5-bf0c-a9d0eff611c3)


![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/fd1e9f9d-271e-4ed2-9519-1947d73ebbe0)


   
   
   Install Git Bash and connect it to AWS Code Commit. Clone the repo (      ) to your git bash and push the vulnearable application to AWS Code Commit. 
  

Psuh code from Git to AWS Code Commit

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/de74f72b-e1d7-49ed-b793-1e58cde77f5c)




 Write a BuildSpec YAML file for the Application in AWS
   
   ![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/00195393-3863-454b-ad14-6f1cc8fd1389)
   
   
   Create a SonarCloud A ccount and intergrate it within AWS DevSecOps pipeline using BuildSpec YAML 
   
   
 ![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/2271287b-5be4-4ae2-ad2e-a68e1e65e5dc)
 ![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/7e4b8179-ab5d-4a1c-9023-f89d133472aa)



Write your Terraform Script to install Jenkins

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/7f9bef8d-0a29-45eb-9cce-d00702ceeaf6)


![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/e4ed3ed1-cbb0-4235-85f6-435891a92cc9)


Check if Jenkins is running

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/46d1348c-4818-4d85-97b1-9435c3fd000c)

Install All Plugin

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/97a0aa0a-a749-481e-96ff-4d0ecb05d18c)


Populate Code coverage by moving the Securirty tokens to AWS Secrets Manager from Build Pipeline. Implement Quality Gate for SonarCloud and run the pipeline

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/5cfd93cd-debf-45dd-b00e-e0589041e68f)


Run the Pipeline 


![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/b8839f9a-0605-42b2-9e83-ea73ba72be93)

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/3f7368be-dc5a-45cd-86b7-a24ae03bd89d)





Create Synk Account 

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/21457a3a-6660-436a-9a52-74a1293043d9)


![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/5aa4954f-d0a0-491b-949d-927d042c5fdc)




intergrate Synk to the Pipeline and wriete a Declarative file to Run a SCA scan

![image](https://github.com/iamdeborah-Q/Devsecops-Jenkins-k8s-Terraform-AWS/assets/122198373/5c728039-df92-4909-9caf-a01679f22a8c)




