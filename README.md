![Travis CI Status](https://travis-ci.org/YakDriver/terraform-aws-provider-static-checks.svg?branch=master)
# terraform-aws-provider-static-checks

This repo shows the current state of static checks in the Terraform AWS provider Go code. This repo uses the (awsproviderlint)[https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint] and rebuilds daily.

# Checks
## AWSAT001

### 
Count: 0
## AWSAT002

### 
Count: 81
[List matches](./results/AWSAT002.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_eip_association_test.go:467:49: AWSAT002: AMI IDs should not be hardcoded`

## AWSAT003

### 
Count: 763
[List matches](./results/AWSAT003.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/structure_test.go:529:42: AWSAT003: regions should not be hardcoded, use aws_region and aws_availability_zones data sources instead`

## AWSAT004

### 
Count: 0
## AWSAT005

### 
Count: 214
[List matches](./results/AWSAT005.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_lb_listener_rule_test.go:3458:21: AWSAT005: avoid hardcoding an AWS partition in an ARN, instead use the aws_partition data source`

## AWSAT006

### 
Count: 507
[List matches](./results/AWSAT006.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_lambda_function_test.go:2435:21: AWSAT006: avoid hardcoding AWS partition DNS suffixes, instead use the aws_partition data source`

## AWSR001

### 
Count: 0
## AWSR002

### 
Count: 0
