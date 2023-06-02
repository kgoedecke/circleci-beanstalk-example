# CircleCI 2.0 Elastic Beanstalk Example
This example shows how to deploy to AWS Elastic Beanstalk (EBS) using [CircleCI 2.0](https://circleci.com/docs/2.0/). 

# Overview
- Continuous Integration of Node app to Beanstalk using CircleCI 2.0
- Multiple Environment deployment: `master` and `develop` to deploy to production and staging Beanstalk environment
- Easily appliable for other platforms/languages
- Support Bitbucket or Github

# Requirements
- The environments in Beanstalk need to be setup already, please follow this guide provided by AWS on [Creating an AWS Elastic Beanstalk Environment](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/using-features.environments.html)
- API credentials for your AWS account, see [Creating an AWS Elastic Beanstalk Environment](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_access-keys.html#Using_CreateAccessKey)
- Github or Bitbucket account
- CircleCI linked to Github or Bitbucket

# Usage
1. Connect CircleCI to your Git
2. Spin up your Beanstalk environment either using the AWS Management Console or the AWS CLI
3. Replace the environment name in `.circleci/config.yml` with your Beanstalk environment name
4. Replace the environment and application name in `.elasticbeanstalk/config.yml`
5. Change the platform (Node, PHP, ...) and AWS Region in `.elasticbeanstalk/config.yml` if needed
6. Push to your master branch to trigger the CircleCI build

For more details see the tutorial below.

# Tutorial
[KevinGoedecke.com - How to deploy to Beanstalk using CircleCI 2.0](https://kevingoedecke.com/2018/03/12/circleci-2-0-beanstalk-example-tutorial/)
