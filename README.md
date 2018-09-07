# moqui-beanstalk
creates elastic beanstalk application and uploads moqui-plus-runtime
using
"64bit Amazon Linux 2018.03 v2.7.2 running Java 8"

1] Requires credentials file (no extension) at: ~/.aws/credentials
contents of this file are 3 lines:
[default]
aws_access_key_id=[AWS IAM user access key id]
aws_secret_access_key=[AWS IAM user access key]

(make sure the AWS IAM user has elastic beanstalk permissions, such as: AWSElasticBeanstalkFullAccess)

2] Requires config file for region (no extension) at: ~/.aws/config
contents of this file are 2 lines:
[default]
region = us-east-1

3] requires your moqui-plus-runtime application zip file to be defined at:
S3Service.java file
private variables for _filePath and _fileName
