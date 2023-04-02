# Setting up AWS

```
aws sts get-caller-identity
export AWS_ACCESS_KEY_ID=
export AWS_SECRET_ACCESS_KEY=
```
Remember to make sure the environment variables are set in control panel, environment variables.
## IAM Roles for services

we need to make an IAM role for our EC2 instance , assign permissions to give access

Firstly go to Identity and Access Management (IAM) in AWS and click on Roles. 
A role can be made for EC2 with IAMReadOnlyAccess

## IAM Guidelines and Best Practicess

Don't use the root account except for AWS account setup
One physical user = One AWS user
Assign users to groups and assign permissions to groups
Create a strong password policy
Use and enforce the use of Multi Factor Authentication (MFA)
Create and use Roles for giving permissions to AWS services