# Create AWS infrastructure

* VPC
* 2 Public subnets in 2 different AZs
* Internet Gateway
* Routing tables

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
aws cloudformation create-stack --capabilities CAPABILITY_IAM --stack-name aws-cfn --template-body file://./vpc.yml
```

```bash
aws cloudformation update-stack --stack-name aws-cfn --template-body file://./vpc.yml
```

```bash
aws cloudformation delete-stack --stack-name aws-cfn
```


## Image

![image](https://user-images.githubusercontent.com/66196388/183374536-9d1c61f2-f9ea-43f0-9304-00570cb4a144.png)
