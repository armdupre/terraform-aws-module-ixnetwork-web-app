# module-ixnetwork-web-app/aws

## Description
Terraform module for IxNetwork Web application deployment on Amazon Web Services

## Deployment
This module creates a single instance having a single network interface.

## Usage
```tf
module "App" {
	source  = "armdupre/module-ixnetwork-web-app/aws"
	Eth0SecurityGroupId = aws_security_group.PublicSecurityGroup.id
	Eth0SubnetId = aws_subnet.PublicSubnet.id
}
```