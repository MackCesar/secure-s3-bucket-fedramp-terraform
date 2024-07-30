# AWS and Azure Terraform Scripts for FISMA/FedRAMP Compliance

This repository contains Terraform scripts to set up AWS and Azure environments with configurations that align with FISMA and FedRAMP compliance standards. The scripts demonstrate how to secure AWS S3 buckets and Azure Storage Accounts with encryption, logging, access controls, and versioning.

## AWS Setup

### Requirements
- Terraform installed
- AWS CLI installed and configured
- An AWS account

### Instructions
1. Clone this repository.
2. Navigate to the `aws` directory.
3. Initialize Terraform:
   ```
   terraform init
   ```
   
4. Apply the Terraform configuration:
	```
	terraform apply
	```
 
### AWS Resources Created

	* 	S3 bucket with server-side encryption
	* 	S3 bucket policy to enforce HTTPS access
	* 	S3 access logging enabled
	* 	S3 versioning enabled
	* 	IAM role with S3 access policy

### Azure Setup

### Requirements

	* 	Terraform installed
	* 	Azure CLI installed and configured
	* 	An Azure account

### Instructions

	1.	Clone this repository.
	2.	Navigate to the azure directory.
	3.	Initialize Terraform:

	```
	terraform init
	```
 
	4.	Apply the Terraform configuration:
	```
	terraform apply 
	```

### Azure Resources Created

	* 	Azure Resource Group
	* 	Azure Storage Account with encryption and network rules
	* 	Storage account diagnostics and logging enabled
	* 	Storage account versioning enabled

### Compliance Notes

These Terraform scripts include basic setups for FISMA and FedRAMP compliance. Depending on your specific requirements, additional configurations may be necessary, such as more granular IAM roles, VPC setups, and additional logging and monitoring configurations.

### Contribution

Feel free to open issues or pull requests if you have suggestions for improvements or additional features.

### License

This project is licensed under the MIT License.
