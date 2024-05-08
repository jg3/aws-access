## aws-access/please
This is a script to easily configure and enable AWS Console Role Switching.

1. log into the AWS Console for account you want to provide access TO.
2. Open CloudShell in the AWS Console, paste in this string:  
` bash <(curl -s https://raw.githubusercontent.com/jg3/aws-access/main/please)`
3. You will be prompted to put in the AWS Account ID to allow access FROM, the rest is automatic.

WARNING:  
This script enables full access to your account, so be sure the FROM account is well protected (e.g. with MFA).

Note(s):  
. there's a way to include a check for MFA in the Role JSON, but it didn't work in my SAML envoronment.  
. it would likewise be possible to create or attach a policy with something less than AdministratorAccess.
