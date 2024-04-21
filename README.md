# CloudFormation Infrastructure as Code (IaC) for AWS

This repository contains a collection of AWS CloudFormation templates automated whit GitHub Actions for deploying and managing AWS resources.

## Main Features

- **Automated Deployment**: Deploy CloudFormation templates automatically with GitHub Actions.
- **Continuous Integration**: Validate CloudFormation templates automatically with GitHub Actions.
- **Parameterized Templates**: Customize CloudFormation templates with parameters.
- **Secure**: Securely store and access sensitive information with GitHub Secrets.
- **Reusable**: Use nested stacks to reuse template code.

## Automated Deployment

This repository uses GitHub Actions to automatically deploy CloudFormation templates to AWS. The deployment workflow is defined in the `.github/workflows/deploy.yml` file. It uses the `aws-actions/configure-aws-credentials` action to configure AWS credentials and the `aws-cloudformation-github-deploy` action to deploy CloudFormation templates.

The workflow is triggered on every push to the `templates` directory. It validates the CloudFormation templates and deploys them to AWS.

## Continuous Integration

This repository uses GitHub Actions to automatically validate CloudFormation templates. The validation workflow uses the `cfn-lint` tool to validate the CloudFormation templates before deployment.

## Parameterized Templates

This repository uses parameterized CloudFormation templates to customize the resources that are created. The parameters are defined in the `parameters.json` file. The parameters are passed to the CloudFormation templates during deployment.

## Secure
