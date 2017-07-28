# ansikube
Kubernetes deployed with Ansible on AWS

## AWS Creation
- vpc
- public subnet
- route table
- internet gateway
- iam role
- s3 bucket
- security groups
- elb
- launch configuration
- autoscaling group

## Kubernetes
- ami coreos
- configuration with cloud-config
- autoscaling group for controller and worker
- etcd and controller pods in same instance
- elb for etcd and controller pods

## Issues
- Flanneld connection to etcd with openssl certificate
- Teardown error with removing the elb's security group

## Todo
- update state for create new launch configuration when ami/user-data/security groups changed
- get last coreos ami
- refactor name for each state