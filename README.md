## aws-access/please
This is a script to easily configure and enable AWS Console Role Switching.

1. Log into the AWS Console for account you want to provide access TO.
3. Open CloudShell in the AWS Console, paste in this string:  
` bash <(curl -s https://raw.githubusercontent.com/jg3/aws-access/main/please) `
4. You will be prompted to put in the AWS Account ID to allow access FROM, the rest is automatic.
5. Log out of the AWS account to provide access TO.
6. Log into the AWS account to get access FROM.
7. Paste the URL provided by the script into your browser.

WARNING:  
This script enables full access to your account, so be sure the FROM account is well protected (e.g. with MFA).

Note(s):  
. there's a way to include a check for MFA in the Role JSON, but it didn't work in my SAML envoronment.  
. it would likewise be possible to create or attach a policy with something less than AdministratorAccess.

<img width="663" alt="AwsSwitchRole" src="https://github.com/jg3/aws-access/assets/2963153/681eacb7-0e51-4824-ac1a-fb17d23c4b2f">
