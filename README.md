# Okta-Integration-with-AWS-Identity-Center

#### Topics Covered:
- How to integrate Okta with AWS IAM Identity Center (successor to AWS SSO)
- How to push groups and users from Okta to AWS
- How to assign permissions in AWS to the pushed users

###### What is Okta?
Okta provides easy, secure access for your workforce so you can focus on other strategic priorities—like reducing costs, and doing more for your customers.

It’s an enterprise-grade, identity management service, built in the cloud for the cloud, but also compatible with many on-premises applications. With Okta, IT can manage any employee’s access to any application or device.

The Okta solution was born of the unique challenges of how technology has grown and shifted in the growing diversity of devices, identity issues, security, employee mobility, vendor partnership, and the exponential growth of unique application options.

Okta features include Provisioning, Single Sign-On (SSO), Active Directory (AD) and LDAP integration, the centralized de-provisioning of users, multifactor authentication (MFA) and flexible policies for organization security and control.

All of these functions are brought together through a network of pre-integrated applications called the  . The OIN provides diverse integration options, enabling SSO login for every app your users need to access during their workday.

In order to enable customers and partners to address every identity use case, we’ve built a set of modular components, called Platform Services, which can be combined to build new features and tailored experiences faster. These Platform Services are available in Okta’s packaged products, APIs, and SDKs.

###### Why Okta?
When users access AWS Resources, organizations must make sure that the right people can access the right Resources in a secure way. Users can be employees, partners or customers. Their source of truth are HR Systems, AD or LDAP directories, Self Service Registration or Identity Providers. Using the right source of truth is critical for Organizations to automate the Joiner-Mover-Leaver Process:

- Joiner: A new user joins the organization. Okta provides automated Birthright Access to AWS and other Applications to make them as productive as possible on their first day.
- Mover: As users change their job or role, get promoted, change their name due to marriage, or go on leave of absence. Okta keeps the connected systems in sync and provides the right access.
- Leaver: At the end of the lifecycle, users leave immediately, time-based, scheduled by the HR-System, or by just deactivation them in an AD or LDAP directory. Okta deprovisions the access to keep the systems secure.

###### The integration of Okta & AWS IAM Identity Center is straight forward. You create in Okta the AWS IAM Identity Center Application and configure the SSO and Provisioning.
- Okta provides over 7500 pre-build integrations with the Okta Integration Network (OIN) and the AWS IAM Identity Center Integration is just one of them

##### Create AWS IAM Identity Center Application (Steps)
1. Sign in to the Okta admin dashboard, expand Applications, then select Applications.
2. On the Applications page, choose Browse App Catalog.
3. In the search box, type AWS IAM Identity Center, select the app to add the IAM Identity Center app.
4. Select the Sign On tab.
5. Under SAML Signing Certificates, select Actions, and then select View IdP Metadata. A new browser tab opens showing the document tree of an XML file. Select all of the XML from ```<md:EntityDescriptor>``` to ```</md:EntityDescriptor>``` and copy it to a text file.
6. Save the text file as ```metadata.xml```.

###### Note: AWS Organization is mandatory to activate AWS IAM Identity Center. If you don’t have one when you activate AWS IAM Identity Center, you might be prompted to create an AWS Organization. You can find more detailed information on how to configure AWS organization in the link below: AWS: Creating and configuring an organization




