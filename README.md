![Travis CI Status](https://travis-ci.org/YakDriver/terraform-aws-provider-static-checks.svg?branch=main)
# terraform-aws-provider-static-checks

This repo shows the current state of static checks in the Terraform AWS provider Go code. This repo uses the (awsproviderlint)[https://github.com/terraform-providers/terraform-provider-aws/tree/main/awsproviderlint] and rebuilds daily.

# Checks
## AWSAT001

### 
Count: 0
## AWSAT002

### 
Count: 81
[List matches](./results/AWSAT002.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_spot_fleet_request_test.go:2040:73: AWSAT002: AMI IDs should not be hardcoded`

## AWSAT003

### 
Count: 763
[List matches](./results/AWSAT003.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_lb_test.go:1662:21: AWSAT003: regions should not be hardcoded, use aws_region and aws_availability_zones data sources instead`

## AWSAT004

### 
Count: 0
## AWSAT005

### 
Count: 214
[List matches](./results/AWSAT005.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_storagegateway_working_storage_test.go:36:14: AWSAT005: avoid hardcoding an AWS partition in an ARN, instead use the aws_partition data source`

## AWSAT006

### 
Count: 508
[List matches](./results/AWSAT006.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_flow_log_test.go:612:55: AWSAT006: avoid hardcoding AWS partition DNS suffixes, instead use the aws_partition data source`

## AWSR001

### 
Count: 0
## AWSR002

### 
Count: 0
## AT*

### 
Count: 192
[List matches](./results/AT*.txt)

Example: `    	enable AT002 analysis`

## README_header.md

### 
Count: 192
[List matches](./results/R*.txt)

Example: `  -S026`

## README.md

### 
Count: 192
[List matches](./results/S*.txt)

Example: `    	write CPU profile to this file`

## S*

### 
Count: 192
[List matches](./results/V*.txt)

Example: `  -S010`

## V*

### 
Count: 
