[![Build Status](https://img.shields.io/travis/AntiPhotonltd/list-aws-service-availability-by-region/master.svg)](https://travis-ci.org/AntiPhotonltd/list-aws-service-availability-by-region)
[![Software License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE.md)
[![Release](https://img.shields.io/github/release/AntiPhotonltd/list-aws-service-availability-by-region.svg)](https://github.com/AntiPhotonltd/list-aws-service-availability-by-region/releases/latest)
[![Github commits (since latest release)](https://img.shields.io/github/commits-since/AntiPhotonltd/list-aws-service-availability-by-region/latest.svg)](https://github.com/AntiPhotonltd/list-aws-service-availability-by-region/commits)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/AntiPhotonltd/list-aws-service-availability-by-region.svg)](https://github.com/AntiPhotonltd/list-aws-service-availability-by-region)
[![GitHub contributors](https://img.shields.io/github/contributors/AntiPhotonltd/list-aws-service-availability-by-region.svg)](https://github.com/AntiPhotonltd/list-aws-service-availability-by-region)

List AWS Service Availability by Region
=========

A python script to get a list of all services and their availability per region.

You can selectively include or excludes regions and services from the search result.

## Simple Usage

```
./list-aws-service-availability-by-region.py
```

## Command Line Options

```

usage: list-aws-service-availability-by-region.py [-h] [-i]
                                                  [-e EXCLUDE_REGION]
                                                  [-E EXCLUDE_SERVICE] [-n]
                                                  [-r] [-s SEARCH_REGION]
                                                  [-S SEARCH_SERVICE]

List AWS Service Availability by Region

optional arguments:
  -h, --help            show this help message and exit
  -i, --case-insensitive
                        Make search/exclude matching case insensitive
  -e EXCLUDE_REGION, --exclude-region EXCLUDE_REGION
                        The region to exclude from the results
  -E EXCLUDE_SERVICE, --exclude-service EXCLUDE_SERVICE
                        The service to exclude from the results
  -n, --no-results      Do not show the final table of results
  -r, --use-regions     Use aws region names instead of country names
  -s SEARCH_REGION, --search-region SEARCH_REGION
                        The region to search the results for
  -S SEARCH_SERVICE, --search-service SEARCH_SERVICE
                        The service to search the results for
```

## Example output

This is an example of the first 3 regions.

```
+-------------------------------------------------------+-------------------+------+--------+
|                                                       | Northern Virginia | Ohio | Oregon |
+-------------------------------------------------------+-------------------+------+--------+
|                   Alexa for Business                  |         Y         |  N   |   N    |
+-------------------------------------------------------+-------------------+------+--------+
|                   Amazon API Gateway                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  Amazon AppStream 2.0                 |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     Amazon Athena                     |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|            Amazon Aurora - MySQL-compatible           |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|         Amazon Aurora - PostgreSQL-compatible         |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                      Amazon Chime                     |         Y         |  N   |   N    |
+-------------------------------------------------------+-------------------+------+--------+
|                 Amazon Cloud Directory                |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   Amazon CloudSearch                  |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   Amazon CloudWatch                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                Amazon CloudWatch Events               |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                 Amazon CloudWatch Logs                |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     Amazon Cognito                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   Amazon Comprehend                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               Amazon Comprehend Medical               |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     Amazon Connect                    |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon DeepLens                    |         Y         |  N   |   N    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon DynamoDB                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                Amazon EC2 Auto Scaling                |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|        Amazon Elastic Container Registry (ECR)        |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|         Amazon Elastic Container Service (ECS)        |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
| Amazon Elastic Container Service for Kubernetes (EKS) |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   Amazon ElastiCache                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|            Amazon Elastic Block Store (EBS)           |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|           Amazon Elastic Compute Cloud (EC2)          |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|    Amazon Elastic Compute Cloud (EC2) A1 Instances    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|    Amazon Elastic Compute Cloud (EC2) C5n Instances   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|            Amazon Elastic File System (EFS)           |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                Amazon Elastic Graphics                |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                Amazon Elastic Inference               |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                Amazon Elastic MapReduce               |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|              Amazon Elasticsearch Service             |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               Amazon Elastic Transcoder               |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon FreeRTOS                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                       Amazon FSx                      |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon GameLift                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     Amazon Glacier                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon GuardDuty                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon Inspector                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|             Amazon Kinesis Data Analytics             |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|              Amazon Kinesis Data Firehose             |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|              Amazon Kinesis Data Streams              |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|              Amazon Kinesis Video Streams             |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                       Amazon Lex                      |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon Lightsail                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                Amazon Machine Learning                |         Y         |  N   |   N    |
+-------------------------------------------------------+-------------------+------+--------+
|                      Amazon Macie                     |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               Amazon Managed Blockchain               |         Y         |  N   |   N    |
+-------------------------------------------------------+-------------------+------+--------+
|                Amazon Mobile Analytics                |         Y         |  N   |   N    |
+-------------------------------------------------------+-------------------+------+--------+
|                       Amazon MQ                       |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     Amazon Neptune                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon Pinpoint                    |         Y         |  N   |   N    |
+-------------------------------------------------------+-------------------+------+--------+
|                      Amazon Polly                     |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   Amazon QuickSight                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon Redshift                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                Amazon Rekognition Image               |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                Amazon Rekognition Video               |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|        Amazon Relational Database Service (RDS)       |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon SageMaker                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|             Amazon SageMaker Ground Truth             |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  Amazon SageMaker Neo                 |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon SimpleDB                    |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|           Amazon Simple Email Service (SES)           |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|        Amazon Simple Notification Service (SNS)       |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|           Amazon Simple Queue Service (SQS)           |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|           Amazon Simple Storage Service (S3)          |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|          Amazon Simple Workflow Service (SWF)         |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon Sumerian                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   Amazon Transcribe                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon Translate                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|           Amazon Virtual Private Cloud (VPC)          |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon WorkDocs                    |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    Amazon WorkMail                    |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   Amazon WorkSpaces                   |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|         Amazon WorkSpaces Application Manager         |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|           AWS Application Discovery Service           |         N         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                      AWS AppSync                      |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    AWS Auto Scaling                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                       AWS Batch                       |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                AWS Certificate Manager                |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS Cloud Map                     |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   AWS CloudFormation                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                       AWS Cloud9                      |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                      AWS CloudHSM                     |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS CloudHSM Classic                 |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS CloudTrail                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS CodeBuild                     |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS CodeCommit                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS CodeDeploy                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    AWS CodePipeline                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                      AWS CodeStar                     |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                       AWS Config                      |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|             AWS Database Migration Service            |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   AWS Data Pipeline                   |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                      AWS DataSync                     |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS DeepRacer                     |         Y         |  N   |   N    |
+-------------------------------------------------------+-------------------+------+--------+
|                    AWS Device Farm                    |         N         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   AWS Direct Connect                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                 AWS Directory Service                 |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                 AWS Elastic Beanstalk                 |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               AWS Elemental MediaConnect              |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               AWS Elemental MediaConvert              |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                AWS Elemental MediaLive                |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               AWS Elemental MediaPackage              |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                AWS Elemental MediaStore               |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               AWS Elemental MediaTailor               |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                      AWS Fargate                      |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Firewall Manager                 |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                 AWS Global Accelerator                |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                        AWS Glue                       |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS Greengrass                    |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    AWS IoT 1-Click                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   AWS IoT Analytics                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                      AWS IoT Core                     |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                AWS IoT Device Defender                |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               AWS IoT Device Management               |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               AWS Key Management Service              |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                       AWS Lambda                      |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Managed Services                 |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    AWS Marketplace                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   AWS Migration Hub                   |         N         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS Mobile Hub                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS OpsWorks Stacks                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|             AWS OpsWorks for Chef Automate            |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|           AWS OpsWorks for Puppet Enterprise          |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|             AWS Personal Health Dashboard             |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS RoboMaker                     |         Y         |  N   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Secrets Manager                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    AWS Security Hub                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|         AWS Serverless Application Repository         |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|              AWS Server Migration Service             |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Service Catalog                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Shield Standard                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Shield Advanced                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   AWS Single Sign-On                  |         Y         |  N   |   N    |
+-------------------------------------------------------+-------------------+------+--------+
|                      AWS Snowball                     |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   AWS Snowball Edge                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                     AWS Snowmobile                    |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                   AWS Step Functions                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Storage Gateway                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                      AWS Support                      |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Systems Manager                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Transit Gateway                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                  AWS Trusted Advisor                  |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                        AWS WAF                        |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|               AWS Well-Architected Tool               |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                       AWS X-Ray                       |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                 Elastic Load Balancing                |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
|                    VM Import/Export                   |         Y         |  Y   |   Y    |
+-------------------------------------------------------+-------------------+------+--------+
```

## Advanced Usage

This is an example of the output when using -S (search service) - again limited to the first 5 regions.

```
./list-aws-service-availability-by-region.py -S 'AWS WAF,AWS Trusted Advisor'
+---------------------+-------------------+------+--------+---------------------+----------+
|                     | Northern Virginia | Ohio | Oregon | Northern California | Montreal |
+---------------------+-------------------+------+--------+---------------------+----------+
| AWS Trusted Advisor |         Y         |  Y   |   Y    |          Y          |    Y     |
+---------------------+-------------------+------+--------+---------------------+----------+
|       AWS WAF       |         Y         |  Y   |   Y    |          Y          |    N     |
+---------------------+-------------------+------+--------+---------------------+----------+
```
## ToDo

- [X] Search by region
- [X] Exclude by region
- [X] Search by service
- [X] Exclude by service
- [X] Make search and exclude accept comma separted lists.
- [X] Partial string matching for search and exclude
- [ ] Validate included / excluded services
- [X] Store the countries per tab so that get_rows_by_service_wrapper is dynamic (number of tables and columns per table)
