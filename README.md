# Serverless Framework React App Deployment with AWS S3 and CloudFront

----

This is a sample project to demonstrate the use case of the Serverless Framework to deploy a ReactJS app to S3 and serve it with CloudFront, 
using a GitHub workflow for continuous integration and continuous deployment (CI/CD). The project also includes the use of Prettier and ESLint for code formatting, 
and Husky with pre-commit hooks for automated linting before commits are made. 
This ensures that the code follows consistent formatting and catches potential errors before they are pushed to the repository. 
Overall, this project showcases the benefits of using Serverless Framework and related tools to streamline the deployment and maintenance of ReactJS apps on AWS.

----

## GitHub Workflow
The GitHub workflow for this project deploys a dev version when a push is made to the dev branch. 
For master or release branch, a manual pipeline trigger needs to be added.

## Configuration
The Serverless Framework configuration file, `serverless.yml`, is located at the root of the project. It defines the AWS resources used for the application, 
including S3 buckets and CloudFront distributions. The configuration also specifies the plugins used by the project, 
including the serverless-s3-sync and serverless-cloudfront-invalidate plugins used to deploy the application to AWS.

## Code Formatting and Linting
This project uses Prettier and ESLint for code formatting and Husky with pre-commit hooks for linting. 
The `.prettierrc` and `.eslintrc.json` files in the project root define the code formatting and linting rules used by the project.
