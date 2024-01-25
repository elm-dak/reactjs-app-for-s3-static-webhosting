This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app) & React Pipeline with AWS CodeStar and Terraform Deployment.

### Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `yarn build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify


### This project demonstrates setting up a continuous integration and continuous deployment (CI/CD) pipeline for a React application using AWS services such as AWS CodeStar for project management and AWS CodePipeline for automating the build, test, and deployment process. Additionally, the deployment is orchestrated using Terraform for infrastructure as code (IaC).

### Overview
The project utilizes the following AWS services:

AWS CodeStar: For project creation, management, and collaboration.
AWS CodePipeline: For automating the CI/CD pipeline.
Terraform: For infrastructure provisioning and deployment.
Prerequisites
Before getting started, ensure you have the following prerequisites:

AWS account with appropriate permissions to create and manage resources.
Terraform installed locally. (Installation Guide)
Node.js and npm installed for React application development.
Setup
Clone the Repository:

bash
Copy code
git clone <repository_url>
cd <repository_directory>
Install Dependencies:

Copy code
npm install
AWS CodeStar Setup:

Follow the instructions to create a new AWS CodeStar project for your React application.
Configure AWS CodePipeline:

Set up a new pipeline in AWS CodePipeline, configuring the source, build, and deployment stages as required.
Terraform Setup:

Ensure you have AWS credentials set up locally (either via ~/.aws/credentials or environment variables).
Navigate to the terraform directory.
Initialize Terraform:
csharp
Copy code
terraform init
Deployment:

Deploy the infrastructure using Terraform:
Copy code
terraform apply
Usage
Development:

Make changes to your React application code.
Test locally.
Commit changes and push to the configured Git repository.
CI/CD Pipeline:

AWS CodePipeline will automatically trigger on code changes.
Pipeline stages will execute: source, build, and deployment.
Monitor the pipeline in the AWS Management Console for status and logs.
Customization
Pipeline Configuration:

Modify the AWS CodePipeline configuration (buildspec.yml) to customize the build and deployment process.
Infrastructure:

Adjust the Terraform configuration (terraform/*.tf) to customize AWS resources and deployment settings.
Cleanup
To avoid ongoing charges, ensure to clean up the AWS resources:

Destroy Infrastructure:

Copy code
terraform destroy
Delete AWS CodeStar Project:

Navigate to AWS CodeStar dashboard and delete the project.
Troubleshooting
Refer to AWS documentation for troubleshooting AWS CodeStar, AWS CodePipeline, and Terraform-related issues.

### Resources
AWS CodeStar Documentation
AWS CodePipeline Documentation
Terraform Documentation



