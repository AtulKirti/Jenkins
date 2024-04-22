Node.js Jenkins Pipeline

This Jenkins pipeline is designed to test Node.js applications using Docker as the execution environment. Below is a brief overview of the setup:

Prerequisites
Jenkins installed and configured
Docker installed on the Jenkins server
Node.js installed on the Docker image
Usage
Clone Repository: Clone this repository to your Jenkins server.
Configure Jenkins Pipeline
Create a new pipeline job in Jenkins.
Configure the pipeline to use the Jenkinsfile provided in this repository.
Pipeline Execution
When the pipeline job is triggered, Jenkins will use the Docker agent configured in the pipeline.
The Docker agent will pull the node:16-alpine image if not already available locally.
The pipeline will execute the Test stage, which runs the command node --version to verify the Node.js version installed in the Docker container.
View Results
Check the console output of the pipeline job in Jenkins to see the Node.js version printed by the Test stage.
Notes
Ensure Docker is properly configured and accessible to Jenkins.
Customize the pipeline stages and steps as per your project requirements.
References
Jenkins Documentation
Docker Documentation
Node.js Documentation
