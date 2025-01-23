AWS resources for the project: S3, StepFunctions, ECS, EventBridge, ECR

Steps for Implementation
Prerequisites:
-AWS CLI installed and configured with appropriate credentials.
-Docker installed and operational.
-Administrative access to the AWS account. 

1- Create the S3 bucket to storage the tables
2- Authenticate with Amazon ECR
    - create the images and register
23- Build and Push Docker Images
    - Create the ECS cluster and input the image created
    - Make sure the permission policies are set: AmazonECSTaskExecutionRolePolicy, AmazonS3FullAccess, CloudWatchLogsFullAccess
4- Set Up EventBridge Rule
    - Create the Rule as event-pattern.json
5- Create ECS Task Definitions
6- Build the Step Functions Workflow