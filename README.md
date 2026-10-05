# ☁️ AWS Services

A comprehensive AWS reference covering services, architecture, cloud concepts, security, DevOps, networking, databases, storage, AI/ML, containers, serverless, Terraform, AWS CLI, certifications, projects, and interview preparation.

---

 ## 📖 About

 **AWS Services Reference** is an open-source learning and reference repository for **Amazon Web Services (AWS)**.

 The goal of this project is to provide a structured place to learn and quickly reference AWS services and cloud concepts without having to search through multiple resources.

 The repository covers:

 - ☁️ AWS Services
- 🏗️ Cloud Architecture
- 🌐 Networking
- 🔐 Security & Identity
- 🗄️ Storage & Databases
- 💻 Compute
- 📦 Containers
- ⚡ Serverless
- 🚀 DevOps & CI/CD
- 🤖 AI & Machine Learning
- 📊 Analytics
- 💰 Cost Optimization
- 🛠️ AWS CLI
- 🏗️ Terraform & Infrastructure as Code
- 🎓 AWS Certifications
- 🧪 Hands-on Projects
- 💼 Interview Preparation
- 🔧 Troubleshooting
- 📚 AWS Best Practices

---

 # 📚 Contents

 - AWS Services
- AWS Architecture
- AWS CLI
- Terraform
- CloudFormation
- Networking
- Security
- DevOps
- Containers & Kubernetes
- Serverless
- AI & Machine Learning
- Cost Optimization
- Well-Architected Framework
- Certifications
- Hands-on Projects
- Service Comparisons
- Troubleshooting
- Interview Preparation
- Learning Roadmap
- Repository Structure
- Contributing
- Disclaimer

---

 # ☁️ AWS Services

 The central part of this repository is the AWS service catalog.

 👉 **View the complete AWS Services list**

 Services are organized into categories such as:

 | Category | Examples |
| --- | --- |
| Compute | EC2, Lambda, Batch, Lightsail |
| Containers | ECS, EKS, ECR |
| Storage | S3, EFS, FSx, Glacier |
| Databases | RDS, Aurora, DynamoDB, Neptune |
| Networking | VPC, Route 53, CloudFront, API Gateway |
| Security | IAM, KMS, WAF, Shield, GuardDuty |
| Management | CloudWatch, CloudTrail, CloudFormation, Config |
| Developer Tools | CodeBuild, CodeDeploy, CodePipeline |
| Machine Learning | SageMaker, Bedrock, Rekognition, Textract |
| Analytics | Athena, Redshift, Glue, EMR, Kinesis |
| Integration | SQS, SNS, EventBridge, Step Functions |
| IoT | IoT Core, Greengrass, IoT SiteWise |
| Web & Mobile | Amplify, AppSync, Device Farm |
| Business Applications | Connect, SES, WorkMail |
| End User Computing | WorkSpaces |
| Game Development | GameLift |

AWS continuously introduces, updates, renames, and retires services and features. Always verify current capabilities and availability using the official AWS documentation.

---

 # 🏗️ AWS Architecture

 Learn how AWS services work together to build real-world systems.

 Architecture topics include:

 - Three-tier applications
- Highly available applications
- Multi-AZ architecture
- Multi-Region architecture
- Serverless architecture
- Microservices
- Event-driven architecture
- Containerized applications
- Data lakes
- Data warehouses
- Disaster recovery
- Business continuity
- Hybrid cloud
- Multi-account AWS architecture

 Example:

```
                         Internet
                            │
                            ▼
                       Route 53
                            │
                            ▼
                       CloudFront
                            │
                            ▼
                          AWS WAF
                            │
                            ▼
                    Application Load
                       Balancer
                            │
                 ┌──────────┴──────────┐
                 ▼                     ▼
              EC2/ECS               EC2/ECS
                 │                     │
                 └──────────┬──────────┘
                            ▼
                           RDS
```

---

 # 💻 AWS CLI

 Learn how to manage AWS resources from the command line.

 Example:

```
aws sts get-caller-identity
```

 List S3 buckets:

```
aws s3 ls
```

 List EC2 instances:

```
aws ec2 describe-instances
```

 List IAM users:

```
aws iam list-users
```

 AWS CLI documentation and examples are available in the `aws-cli/` directory.

---

 # 🏗️ Terraform

 Infrastructure as Code examples using Terraform.

 Topics include:

 - AWS provider
- EC2
- VPC
- S3
- IAM
- RDS
- Lambda
- DynamoDB
- ECS
- EKS
- Terraform modules
- Variables
- Outputs
- State management
- Remote state
- Workspaces

 Example:

```
provider "aws" {
  region = "us-east-1"
}

resource "aws_s3_bucket" "example" {
  bucket = "example-bucket"
}
```

---

 # 📜 CloudFormation

 AWS CloudFormation examples for infrastructure automation.

 Topics include:

 - Templates
- Parameters
- Resources
- Outputs
- Conditions
- Mappings
- Nested stacks
- Stack updates
- StackSets

---

 # 🌐 Networking

 AWS networking documentation covers:

 - Amazon VPC
- Subnets
- Route tables
- Internet Gateway
- NAT Gateway
- Security Groups
- Network ACLs
- VPC Peering
- Transit Gateway
- VPN
- Direct Connect
- Route 53
- CloudFront
- Load Balancers
- API Gateway
- Global Accelerator

 A major focus is understanding how to design secure and highly available AWS networks.

---

 # 🔐 Security

 Security topics include:

 - AWS IAM
- IAM policies
- IAM roles
- Least privilege
- MFA
- AWS KMS
- Secrets Manager
- Security Groups
- Network ACLs
- AWS WAF
- AWS Shield
- GuardDuty
- Inspector
- Macie
- CloudTrail
- AWS Config
- Encryption
- Security monitoring
- Incident response

 ### Security principle

 > **Never commit AWS credentials, access keys, secret keys, passwords, or other sensitive information to this repository.**

---

 # 🚀 DevOps

 DevOps topics include:

 - CI/CD
- CodeBuild
- CodeDeploy
- CodePipeline
- GitHub Actions
- Docker
- ECS
- EKS
- Infrastructure as Code
- Automated testing
- Deployment strategies
- Blue/green deployments
- Canary deployments
- Monitoring

---

 # 📦 Containers & Kubernetes

 Container topics include:

 - Docker
- Amazon ECR
- Amazon ECS
- AWS Fargate
- Amazon EKS
- Kubernetes
- Pods
- Deployments
- Services
- Ingress
- ConfigMaps
- Secrets
- Autoscaling
- Container monitoring

 Example architecture:

```
                    Internet
                       │
                       ▼
                  Load Balancer
                       │
                       ▼
                   Amazon EKS
                 ┌─────┴─────┐
                 ▼           ▼
               Pod         Pod
                 │           │
                 └─────┬─────┘
                       ▼
                    Amazon RDS
```

---

 # ⚡ Serverless

 Serverless topics include:

 - AWS Lambda
- API Gateway
- DynamoDB
- S3
- EventBridge
- SQS
- SNS
- Step Functions
- Serverless architecture
- Event-driven applications

 Example:

```
Client
  │
  ▼
API Gateway
  │
  ▼
Lambda
  │
  ▼
DynamoDB
```

---

 # 🤖 AI & Machine Learning

 AWS AI/ML topics include:

 - Amazon Bedrock
- Amazon SageMaker
- Amazon Rekognition
- Amazon Textract
- Amazon Transcribe
- Amazon Translate
- Amazon Comprehend
- Amazon Polly
- Amazon Lex
- Generative AI
- RAG
- Vector databases
- Embeddings
- AI agents
- Machine learning workflows

 Example project:

```
User
 │
 ▼
API Gateway
 │
 ▼
Lambda
 │
 ▼
Amazon Bedrock
 │
 ▼
Knowledge Base / Vector Store
```

---

 # 💰 Cost Optimization

 AWS cost-management topics include:

 - AWS Billing
- Cost Explorer
- AWS Budgets
- Savings Plans
- Reserved Instances
- Spot Instances
- Resource rightsizing
- S3 storage optimization
- EC2 cost optimization
- Database cost optimization
- Cost monitoring
- Tagging strategies

 ### Important principle

 > Design for both **technical efficiency and financial efficiency**.

---

 # 🏛️ Well-Architected Framework

 AWS architecture should consider the six pillars of the AWS Well-Architected Framework:

 1. **Operational Excellence**
2. **Security**
3. **Reliability**
4. **Performance Efficiency**
5. **Cost Optimization**
6. **Sustainability**

 These principles can be applied when reviewing AWS architectures and production workloads.

---

 # 🎓 AWS Certifications

 Resources can be organized around AWS certification paths.

 ### Foundational

 - AWS Certified Cloud Practitioner

 ### Associate

 - AWS Certified Solutions Architect – Associate
- AWS Certified Developer – Associate
- AWS Certified CloudOps Engineer – Associate

 ### Professional

 - AWS Certified Solutions Architect – Professional
- AWS Certified DevOps Engineer – Professional

 Certification information can change, so always check the current AWS certification catalog before preparing for an exam.

---

 # 🧪 Hands-on Projects

 Practical projects are an important part of this repository.

 ## 🟢 Beginner

 - Host a static website using S3
- Launch an EC2 web server
- Create an IAM role
- Build a VPC
- Deploy a Lambda function
- Create an RDS database
- Configure CloudWatch monitoring

 ## 🟡 Intermediate

 - Build a three-tier application
- Create a serverless REST API
- Lambda + API Gateway + DynamoDB
- Deploy Docker containers to ECS
- Build a CI/CD pipeline
- Configure CloudFront + S3
- Build an event-driven application

 ## 🔴 Advanced

 - Highly available multi-AZ application
- Multi-region architecture
- Kubernetes platform using EKS
- Serverless production architecture
- Microservices platform
- AWS data lake
- Disaster recovery solution
- Multi-account AWS architecture
- Infrastructure as Code platform

---

 # ⚖️ Service Comparisons

 Understand when to choose one AWS service over another.

 Examples:

 | Comparison | Question |
| --- | --- |
| EC2 vs Lambda | Servers or serverless? |
| S3 vs EBS vs EFS | Which storage should I use? |
| RDS vs DynamoDB | Relational or NoSQL? |
| SQS vs SNS | Queue or pub/sub? |
| ECS vs EKS | ECS or Kubernetes? |
| ALB vs NLB | Which load balancer? |
| NAT Gateway vs Internet Gateway | What is the difference? |
| CloudFront vs Global Accelerator | CDN or network acceleration? |
| Secrets Manager vs Parameter Store | How should secrets/configuration be managed? |
| Terraform vs CloudFormation | Which IaC tool should I use? |

---

 # 🔧 Troubleshooting

 Practical troubleshooting guides will cover common AWS problems.

 Examples:

 - EC2 SSH connection failure
- EC2 instance has no internet access
- S3 `AccessDenied`
- IAM permission errors
- Lambda timeout
- Lambda cold starts
- RDS connection failures
- ECS task failures
- EKS pod failures
- DNS resolution problems
- VPC routing problems
- Security Group issues
- CloudWatch logging problems

---

 # 💼 Interview Preparation

 AWS interview topics include:

 ### Fundamentals

 - AWS Regions
- Availability Zones
- IAM
- VPC
- EC2
- S3
- RDS

 ### Networking

 - VPC
- Subnets
- Route tables
- NAT Gateway
- Internet Gateway
- Security Groups
- NACLs
- Load Balancers

 ### Architecture

 - High availability
- Scalability
- Fault tolerance
- Disaster recovery
- Multi-AZ
- Multi-Region

 ### DevOps

 - CI/CD
- Docker
- Kubernetes
- Terraform
- CloudFormation

 ### Scenario Questions

 Examples:

 > How would you design a highly available web application?

 > How would you secure an AWS account?

 > How would you reduce an unexpectedly high AWS bill?

 > How would you migrate an on-premises application to AWS?

 > How would you design a multi-region application?

---

 # 🛣️ AWS Learning Roadmap

```
AWS Fundamentals
        │
        ▼
IAM
        │
        ▼
VPC & Networking
        │
        ▼
EC2
        │
        ├──────────────► S3
        │
        ▼
RDS / DynamoDB
        │
        ▼
Load Balancing
        │
        ▼
Auto Scaling
        │
        ▼
Lambda
        │
        ▼
API Gateway
        │
        ▼
Docker
        │
        ▼
ECS / EKS
        │
        ▼
CloudWatch / CloudTrail
        │
        ▼
Security
        │
        ▼
Terraform
        │
        ▼
CI/CD
        │
        ▼
AWS Architecture
        │
        ▼
Production Projects
```

---

 # 📁 Repository Structure

```
aws-services-reference/
│
├── README.md
├── services.md
├── glossary.md
├── CONTRIBUTING.md
├── LICENSE
│
├── services/
│
├── architecture/
│
├── aws-cli/
│
├── terraform/
│
├── cloudformation/
│
├── networking/
│
├── security/
│
├── devops/
│
├── kubernetes/
│
├── serverless/
│
├── ai-ml/
│
├── cost-optimization/
│
├── well-architected/
│
├── certifications/
│
├── projects/
│
├── interview/
│
├── comparisons/
│
├── troubleshooting/
│
├── best-practices/
│
└── diagrams/
```

---

 # 🤝 Contributing

 Contributions are welcome.

 You can contribute by:

 - Adding AWS service documentation
- Correcting technical information
- Adding architecture diagrams
- Adding AWS CLI examples
- Adding Terraform examples
- Adding CloudFormation examples
- Creating hands-on projects
- Improving explanations
- Adding interview questions
- Reporting outdated information

 Before submitting a contribution, make sure that:

 - Examples are tested where practical.
- No AWS credentials are included.
- No secrets or private information are committed.
- Documentation is written clearly.
- AWS service information is based on reliable sources.

---

 # 🔒 Security

 **Never commit credentials to this repository.**

 Do not commit:

```
.env
.aws/credentials
access keys
secret keys
private keys
passwords
API tokens
```

 If credentials are accidentally exposed, revoke or rotate them immediately.

---

 # 📚 Official Resources

 For authoritative and current information, always refer to the official AWS resources:

 - [AWS](<https://aws.amazon.com/>)
- [AWS Documentation](<https://docs.aws.amazon.com/>)
- [AWS Architecture Center](<https://aws.amazon.com/architecture/>)
- [AWS Well-Architected](<https://aws.amazon.com/architecture/well-architected/>)
- [AWS Training](<https://aws.amazon.com/training/>)
- [AWS Certifications](<https://aws.amazon.com/certification/>)
- [AWS CLI Documentation](<https://docs.aws.amazon.com/cli/>)
- [AWS Pricing](<https://aws.amazon.com/pricing/>)

 # ⚖️ Legal & Disclaimer

 **AWS Services Reference is an independent educational and reference project. It is not affiliated with, endorsed by, sponsored by, or officially connected with Amazon Web Services, Inc. or Amazon.com, Inc.**

 Amazon Web Services, AWS, and AWS product and service names are trademarks of Amazon.com, Inc. or its affiliates. AWS trademarks, logos, icons, documentation, and other AWS-owned intellectual property remain the property of their respective owners.

 This repository contains independently created educational material intended for learning, reference, and general informational purposes. It is not intended to reproduce, replace, or represent official AWS documentation, training, certification material, or professional AWS consulting services.

 AWS services, features, APIs, pricing, quotas, limits, terms, supported regions, and availability may change over time. Information in this repository may become outdated or contain errors. Always consult the official AWS documentation and service-specific terms before relying on information for production systems or making technical, security, or financial decisions.

 Third-party content, trademarks, images, diagrams, code, libraries, and other materials referenced or included in this repository remain subject to their respective owners and applicable licenses. Where required, appropriate attribution and licensing information should be provided.

 **Do not commit AWS credentials, access keys, secret keys, passwords, API tokens, private keys, `.env` files, confidential information, or other sensitive data to this repository.**

 Use of the examples and information in this repository is at your own risk. The maintainers and contributors are not responsible for unexpected AWS charges, data loss, service interruptions, security incidents, or other consequences resulting from the use or misuse of the material, to the maximum extent permitted by applicable law.

 For complete copyright, trademark, licensing, attribution, and intellectual-property information, see `LEGAL.md`.

 ### Official Resources

 - [AWS](<https://aws.amazon.com/>)
- [AWS Documentation](<https://docs.aws.amazon.com/>)
- [AWS Legal](<https://aws.amazon.com/legal/>)
- [AWS Trademark Guidelines](<https://aws.amazon.com/trademark-guidelines/>)
- [GitHub DMCA Policy](<https://docs.github.com/en/site-policy/content-removal-policies/dmca-takedown-policy>)

---

 ### Official Resources

 - [AWS Legal](<https://aws.amazon.com/legal/>)
- [AWS Trademark Guidelines](<https://aws.amazon.com/trademark-guidelines/>)
- [AWS Documentation](<https://docs.aws.amazon.com/>)
- [GitHub DMCA Policy](<https://docs.github.com/en/site-policy/content-removal-policies/dmca-takedown-policy>)

---

 # ⭐ Support

 If this repository helps you learn AWS, consider giving it a ⭐ on GitHub.

 Contributions, corrections, suggestions, and improvements are welcome.

---

 ## ☁️ Learn. Build. Secure. Automate. Scale.

 **AWS Services Reference — Your practical AWS knowledge base.**
