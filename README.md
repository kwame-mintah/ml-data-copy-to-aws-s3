# ML Data Copy to AWS S3

This repository contains data that will be copied into an AWS S3 bucket. The AWS Infrastructure Terraform can be found in this repository [terraform-aws-machine-learning-pipeline](https://github.com/kwame-mintah/terraform-aws-machine-learning-pipeline) and contains the creation of the AWS S3 Bucket, GitHub Action Role etc.

## GitHub Action (CI/CD)

The GitHub Action will checkout the repository and upload specified files to the AWS S3 bucket using the [configure-aws-credentials](https://github.com/aws-actions/configure-aws-credentials/tree/v4.0.1/) action. The following repository secrets need to be set:

| Secret          | Description            |
| --------------- | ---------------------- |
| AWS_REGION      | The AWS Region         |
| AWS_ACCOUNT_ID  | The AWS account ID.    |
| AWS_BUCKET_NAME | The AWS S3 bucket name |

## Data

Data in this repository has been copied from other well know machine learning repositories. Please see `README.md` in sub directory detailing where the data was copied from.
