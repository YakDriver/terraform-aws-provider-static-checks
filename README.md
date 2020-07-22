![Travis CI Status](https://travis-ci.org/YakDriver/terraform-aws-provider-static-checks.svg?branch=main)
# terraform-aws-provider-static-checks

Automatic daily rebuilds! This repo shows the current state of static checks in the Terraform AWS provider Go code. This repo uses the [awsproviderlint](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint) and [tfproviderlint](https://github.com/bflad/tfproviderlint).

# Checks
## awsproviderlint

###  [https
Count: 0
###  [https
Count: 81
[List matches](./results/AWSAT002.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_spot_fleet_request_test.go:1478:73: AWSAT002: AMI IDs should not be hardcoded`

###  [https
Count: 763
[List matches](./results/AWSAT003.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_shield_protection_test.go:530:21: AWSAT003: regions should not be hardcoded, use aws_region and aws_availability_zones data sources instead`

###  [https
Count: 0
###  [https
Count: 214
[List matches](./results/AWSAT005.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_cloudwatch_log_resource_policy_test.go:94:70: AWSAT005: avoid hardcoding an AWS partition in an ARN, instead use the aws_partition data source`

###  [https
Count: 508
[List matches](./results/AWSAT006.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_waf_web_acl_test.go:635:21: AWSAT006: avoid hardcoding AWS partition DNS suffixes, instead use the aws_partition data source`

###  [https
Count: 0
###  [https
Count: 0
## tfproviderlint

###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 16
[List matches](./results/AT004.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_opsworks_stack_test.go:721:21: AT004: provider declaration should be omitted`

###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 17
[List matches](./results/R001.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/opsworks_layers.go:591:10: R001: ResourceData.Set() key argument should be string literal`

###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 64
[List matches](./results/R010.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_sns_topic.go:349:3: R010: prefer d.Get() over d.GetChange() when only using second return value`

###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 126
[List matches](./results/V001.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/validators.go:908:1: V001: custom SchemaValidateFunc should be replaced with validation.StringMatch() or validation.StringDoesNotMatch()`

###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
###  [https
Count: 0
