# Enabling multi\-factor authentication<a name="connect_mfa"></a>

You use the AWS Directory Services Console at [https://console\.aws\.amazon\.com/directoryservicev2/](https://console.aws.amazon.com/directoryservicev2/) to enable multi\-factor authentication for your AD Connector directory\. To enable MFA, you must have an MFA solution that is a Remote authentication dial\-in user service \(RADIUS\) server, or you must have an MFA plugin to a RADIUS server already implemented in your on\-premises infrastructure\. Your MFA solution should implement One Time Passcodes \(OTP\) that users obtain from a hardware device or from software running on a device such as a cell phone\.

RADIUS is an industry\-standard client/server protocol that provides authentication, authorization, and accounting management to enable users to connect to network services\. AWS Managed Microsoft AD includes a RADIUS client that connects to the RADIUS server upon which you have implemented your MFA solution\. Your RADIUS server validates the username and OTP code\. If your RADIUS server successfully validates the user, AWS Managed Microsoft AD then authenticates the user against AD\. Upon successful AD authentication, users can then access the AWS application\. Communication between the AWS Managed Microsoft AD RADIUS client and your RADIUS server require you to configure AWS security groups that enable communication over port 1812\.

For more information, see [Enable multi\-factor authentication for AWS Managed Microsoft AD](https://docs.aws.amazon.com/directoryservice/latest/admin-guide/ms_ad_mfa.html) in the *AWS Directory Service Administration Guide*\.

**Note**  
Multi\-factor authentication is not available for Simple AD directories\.