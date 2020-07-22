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

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_network_interface_attachment_test.go:43:21: AWSAT002: AMI IDs should not be hardcoded`

## AWSAT003

### 
Count: 763
[List matches](./results/AWSAT003.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_config_aggregate_authorization_test.go:169:21: AWSAT003: regions should not be hardcoded, use aws_region and aws_availability_zones data sources instead`

## AWSAT004

### 
Count: 0
## AWSAT005

### 
Count: 214
[List matches](./results/AWSAT005.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_media_store_container_policy_test.go:99:21: AWSAT005: avoid hardcoding an AWS partition in an ARN, instead use the aws_partition data source`

## AWSAT006

### 
Count: 508
[List matches](./results/AWSAT006.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_iam_service_linked_role_test.go:220:20: AWSAT006: avoid hardcoding AWS partition DNS suffixes, instead use the aws_partition data source`

## AWSR001

### 
Count: 0
## AWSR002

### 
Count: 0
## AT001

### 
Count: 0
## AT002

### 
Count: 0
## AT003

### 
Count: 0
## AT004

### 
Count: 16
[List matches](./results/AT004.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/data_source_aws_eip_test.go:221:57: AT004: provider declaration should be omitted`

## AT005

### 
Count: 0
## AT006

### 
Count: 0
## AT007

### 
Count: 0
## AT008

### 
Count: 0
## R001

### 
Count: 17
[List matches](./results/R001.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/data_source_aws_vpc_dhcp_options.go:124:10: R001: ResourceData.Set() key argument should be string literal`

## R002

### 
Count: 0
## R003

### 
Count: 0
## R004

### 
Count: 0
## R005

### 
Count: 0
## R006

### 
Count: 0
## R007

### 
Count: 0
## R008

### 
Count: 0
## R009

### 
Count: 0
## R010

### 
Count: 64
[List matches](./results/R010.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_sns_topic.go:277:3: R010: prefer d.Get() over d.GetChange() when only using second return value`

## R011

### 
Count: 0
## R012

### 
Count: 0
## R013

### 
Count: 0
## R014

### 
Count: 0
## S001

### 
Count: 0
## S002

### 
Count: 0
## S003

### 
Count: 0
## S004

### 
Count: 0
## S005

### 
Count: 0
## S006

### 
Count: 0
## S007

### 
Count: 0
## S008

### 
Count: 0
## S009

### 
Count: 0
## S010

### 
Count: 0
## S011

### 
Count: 0
## S012

### 
Count: 0
## S013

### 
Count: 0
## S014

### 
Count: 0
## S015

### 
Count: 0
## S016

### 
Count: 0
## S017

### 
Count: 0
## S018

### 
Count: 0
## S019

### 
Count: 0
## S020

### 
Count: 0
## S021

### 
Count: 0
## S022

### 
Count: 0
## S023

### 
Count: 0
## S024

### 
Count: 0
## S025

### 
Count: 0
## S026

### 
Count: 0
## S027

### 
Count: 0
## S028

### 
Count: 0
## S029

### 
Count: 0
## S030

### 
Count: 0
## S031

### 
Count: 0
## S032

### 
Count: 0
## S033

### 
Count: 0
## S034

### 
Count: 0
## S035

### 
Count: 0
## S036

### 
Count: 0
## S037

### 
Count: 0
## V001

### 
Count: 126
[List matches](./results/V001.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/validators.go:1153:1: V001: custom SchemaValidateFunc should be replaced with validation.StringMatch() or validation.StringDoesNotMatch()`

## V002

### 
Count: 0
## V003

### 
Count: 0
## V004

### 
Count: 0
## V005

### 
Count: 0
## V006

### 
Count: 0
## V007

### 
Count: 0
## V008

### 
Count: 0
