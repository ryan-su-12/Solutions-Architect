#### IAM - Password Policy
---
- Strong Passwords = Higher Security for account
- In AWS, you can setup a password policy
	- Set minimum password length
	- Require specific character types
	- Allow all IAM users to change their own password
	- Require uses to change their password after some time
	- Prevent Password reuse

#### Multi Factor Authentication - MFA
---
- Users have access to your account and can possibly change configurations or delete resources in your AWS account
- You want to protect your root account and IAM users
- MFA = Password you know + security device you own![[Pasted image 20241221093132.png]]
- So if a password is stolen or hacked, the account is not compromised
**MFA devices in AWS**:
- Virtual MFA device like google authenticator or authy
- Universal 2nd Factor (U2F) security key, could be a physical device
- Hardware Key Fob MFA device
- Hardware key fob MFA device for AWS GovCloud

