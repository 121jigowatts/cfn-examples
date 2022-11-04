# CloudFrontとS3でBasic認証

```sh
aws cloudformation create-stack \
--stack-name s3webhosting-basic-auth \
--template-body file://basic-auth.yaml \
--parameters \
ParameterKey=BucketName,ParameterValue={Bucket Name}
```
