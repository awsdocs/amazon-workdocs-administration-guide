# Prerequisites for Amazon WorkDocs<a name="prereqs"></a>

To set up new Amazon WorkDocs sites, or manage existing sites, you must complete the following tasks\.

**Topics**
+ [Sign Up for AWS](#console_signup)
+ [Create IAM Users and Groups \(Recommended\)](#create_iam_user)
+ [Grant IAM Users Permissions for Amazon WorkDocs](#iam_policies)

## Sign Up for AWS<a name="console_signup"></a>

Your AWS account gives you access to all services, but you are charged only for the resources that you use\.

If you do not have an AWS account, use the following procedure to create one\.

**To sign up for AWS**

1. Open [https://aws\.amazon\.com/](https://aws.amazon.com/) and choose **Create an AWS Account**\.

1. Follow the online instructions\.

Your root account credentials identify you to services in AWS and grant you unlimited use of your AWS resources, such as your Amazon WorkDocs sites\. To allow other users to set up new Amazon WorkDocs sites, or manage existing sites, without sharing your security credentials, use AWS Identity and Access Management \(IAM\)\. We recommend that everyone work as an IAM user, even the account owner\. You should create an IAM user for yourself, give that IAM user administrative privileges, and use it for all your work\. 

## Create IAM Users and Groups \(Recommended\)<a name="create_iam_user"></a>

The AWS Management Console requires your username and password so that the service can determine whether you have permission to access its resources\. We recommend that you avoid using root account credentials to access AWS because root account credentials cannot be revoked or limited in any way\. Instead, use AWS Identity and Access Management \(IAM\) to create an IAM user and add the IAM user to an IAM group with administrative permissions\. This grants the IAM user administrative permissions\. You can then access the AWS Management Console using the credentials for the IAM user\.

If you signed up for AWS but have not created an IAM user for yourself, you can create one using the IAM console\. For more information about creating an IAM user, see [Create individual IAM users](https://docs.aws.amazon.com/IAM/latest/UserGuide/IAMBestPractices.html#create-iam-users) in the *IAM User Guide* guide\.

## Grant IAM Users Permissions for Amazon WorkDocs<a name="iam_policies"></a>

By default, IAM users don't have permissions to manage Amazon WorkDocs resources; you must create an IAM policy that explicitly grants IAM users those permissions, and attach the policy to the specific IAM users or groups that require those permissions\. For more information about IAM policies, see [Permissions and Policies](https://docs.aws.amazon.com/IAM/latest/UserGuide/PermissionsAndPolicies.html) in the *IAM User Guide* guide\.

The following policy statement grants an IAM user full access to Amazon WorkDocs resources\. The policy gives the user access to all Amazon WorkDocs and AWS Directory Service operations, as well as several Amazon EC2 operations that Amazon WorkDocs needs to be able to perform on your behalf\.

```
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Action": [
          "workdocs:*",
          "ds:*",
          "ec2:CreateVpc",
          "ec2:CreateSubnet",
          "ec2:CreateNetworkInterface",
          "ec2:CreateTags",
          "ec2:CreateSecurityGroup",
          "ec2:DescribeVpcs",
          "ec2:DescribeSubnets",
          "ec2:DescribeNetworkInterfaces",
          "ec2:DescribeAvailabilityZones",
          "ec2:AuthorizeSecurityGroupEgress",
          "ec2:AuthorizeSecurityGroupIngress",
          "ec2:DeleteSecurityGroup",
          "ec2:DeleteNetworkInterface",
          "ec2:RevokeSecurityGroupEgress",
          "ec2:RevokeSecurityGroupIngress"
          ],
      "Effect": "Allow",
      "Resource": "*"
    }
  ]
}
```

The following policy statement grants an IAM user read\-only access to Amazon WorkDocs resources\. The policy gives the user access to all of the Amazon WorkDocs `Describe` operations\. Access to the two Amazon EC2 operations are necessary so Amazon WorkDocs can obtain a list of your VPCs and subnets\. Access to the AWS Directory Service `DescribeDirectories` operation is needed to obtain information about your AWS Directory Service directories\.

```
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Action": [
          "workdocs:Describe*",
          "ds:DescribeDirectories",       
          "ec2:DescribeVpcs",
          "ec2:DescribeSubnets"
          ],
      "Effect": "Allow",
      "Resource": "*"
    }
  ]
}
```