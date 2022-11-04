# 指定したIPのみアクセス可能とする

```sh
aws cloudformation create-stack \
--stack-name s3webhosting-ip-allow \
--template-body file://ip-allow.yaml \
--parameters \
ParameterKey=S3BucketName,ParameterValue={Bucket Name} \
ParameterKey=AllowIP,ParameterValue={IP ADDRESS}
```
