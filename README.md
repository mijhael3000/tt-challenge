# TT challenge

This is an example about how to deploy an nginx server with terraform, aws and ansible. 

## Pre-requirements:

To run this code, you need to:

- Install terraform.
- Configure your aws credentials setting up the env variables: **AWS_ACCESS_KEY_ID**
**AWS_SECRET_ACCESS_KEY** or your *~/.aws/credentials* file
- create ssh keys.

## Usage
clone repo:
`git clone git@github.com:mijhael3000/tt-challenge.git`

Init Terraform code
```bash
terraform init
```
Apply terraform code passwing vars with the path to your keys:
```bash
terraform apply -auto-approve -var 'priv_key=your_private_key' -var 'pub_key=your_public.key'
```
