
# Add remote dvc repository hosted in S3
```
dvc remote add -d orange_s3  s3://msc-dev-datalake/datasets/orange
```

## Configure S3 user and check access
This steps need to be done in each  directory with a DVC repository
```
aws configure
```
Requests to input Key and Secret, use the ones obtained from AWS. Leave the rest of the options as default.
```
AWS Access Key ID [****************AGGE]: *****
AWS Secret Access Key [****************QMAO]: *********
Default region name [None]:
Default output format [None]:
```
To verify we have access, IMPORTANT: use the corresponding URL.
```
aws s3 ls s3://msc-dev-datalake/datasets/
```