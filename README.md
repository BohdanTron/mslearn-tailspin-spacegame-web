# Azure Pipelines Project

This project was created to explore and learn Azure Pipelines by building, testing, and deploying applications through a CI/CD pipeline.

## Overview

The pipeline is hosted on [Azure DevOps](https://dev.azure.com/tronbodya/) and can be accessed here.

## Pipeline Workflow

The pipeline is designed to build both the .NET and UI applications, followed by a deployment to Azure App Service.

## Environments

There are three deployment environments configured in the pipeline:

- **Dev:** Automatic deployment when changes are pushed to the release branch.
- **Test:** Automatic deployment after succeeded execution of 'Dev' stage.
- **Staging:** Requires manual approval before deployment.

## Key Features
- **Automated Builds:** Triggers on push events to the release branch, initiating builds for both backend and UI components.
- **Environment-Specific Deployments:** Each environment has dedicated deployment settings to enable targeted deployments.
- **Manual Approvals:** Staging deployment requires manual approval, ensuring only reviewed changes make it to the staging environment.
