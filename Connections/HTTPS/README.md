
# HTTPS Username & Password
1) Create an IAM user with CodeCommitFullAccess.
2) Navigate to the IAM console -> IAM user -> Security Credentials 
3) Select "Generate Credentials" under HTTPS Git credentials for AWS CodeCommit
4) Copy the 'user-name' and 'password'. Else, Download the credentials

Resources: https://docs.aws.amazon.com/codecommit/latest/userguide/setting-up-gc.html#setting-up-gc-account

# HTTPS Credential Helper

1) Configure the machine with the IAM user which has the HTTPS credentials
2) Run the below commands 

```
git config --global credential.helper '!aws codecommit credential-helper $@'
git config --global credential.UseHttpPath true
```

Resources:https://docs.aws.amazon.com/codecommit/latest/userguide/setting-up-https-unixes.html#setting-up-https-unixes-account