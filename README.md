# Create AWS infrastructure

* VPC
* 2 subnets in 2 different AZs
* Internet Gateway
* routing tables

Commands:  

```bash
pip3 install cfn-lint
```

```bash
cfn-lint vpc.yml
```

```bash
aws configure
```

```bash
aws cloudformation create-stack --capabilities CAPABILITY_IAM --stack-name aws-vpc --template-body file://./vpc.yml
```
