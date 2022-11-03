## AWS Lambda Example

This examples shows how to deploy an AWS Lambda function using Terraform only.

To run, configure your AWS provider as described in https://www.terraform.io/docs/providers/aws/index.html


Now one should have a seperate directory and under that directory create  files and named them as:

```
hello_lambda.py
main.tf
outputs.tf
variable.tf
```

Now you should have AWS CLI in your local machine and then configure your AWS as:

```
provider "aws"{
region = "ap-south-1"
access_key = "Your_Access_Key"
secret_key = "Your_Secret_Key"
}
```

Now run the Terraform command to Configure AWS Lambda as:


```
terraform init
```

```
terraform plan
```

```
terraform apply
```

At last if you want to delete the resources to avoid unnecessary charges , you should use:

```
terraform destroy
```


