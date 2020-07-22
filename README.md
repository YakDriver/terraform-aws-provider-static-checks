![Travis CI Status](https://travis-ci.org/YakDriver/terraform-aws-provider-static-checks.svg?branch=main)
# terraform-aws-provider-static-checks

Automatic daily rebuilds! This repo shows the current state of static checks in the Terraform AWS provider Go code. This repo uses the [awsproviderlint](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint) and [tfproviderlint](https://github.com/bflad/tfproviderlint).

# Checks
## awsproviderlint

###  [AWSAT001](https
Count: 0
###  [AWSAT002](https
Count: 81
[List matches](./results/AWSAT002.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/data_source_aws_instance_test.go:517:21: AWSAT002: AMI IDs should not be hardcoded`

###  [AWSAT003](https
Count: 763
[List matches](./results/AWSAT003.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_lb_target_group_test.go:71:23: AWSAT003: regions should not be hardcoded, use aws_region and aws_availability_zones data sources instead`

###  [AWSAT004](https
Count: 0
###  [AWSAT005](https
Count: 214
[List matches](./results/AWSAT005.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/validators_test.go:2561:14: AWSAT005: avoid hardcoding an AWS partition in an ARN, instead use the aws_partition data source`

###  [AWSAT006](https
Count: 508
[List matches](./results/AWSAT006.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_iam_role_test.go:834:21: AWSAT006: avoid hardcoding AWS partition DNS suffixes, instead use the aws_partition data source`

###  [AWSR001](https
Count: 0
###  [AWSR002](https
Count: 0
## tfproviderlint

###  [AT001](https
Count: 0
###  [AT002](https
Count: 0
###  [AT003](https
Count: 0
###  [AT004](https
Count: 16
[List matches](./results/AT004.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_instance_test.go:3386:21: AT004: provider declaration should be omitted`

###  [AT005](https
Count: 0
###  [AT006](https
Count: 0
###  [AT007](https
Count: 0
###  [AT008](https
Count: 0
###  [R001](https
Count: 17
[List matches](./results/R001.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/opsworks_layers.go:591:10: R001: ResourceData.Set() key argument should be string literal`

###  [R002](https
Count: 0
###  [R003](https
Count: 0
###  [R004](https
Count: 0
###  [R005](https
Count: 0
###  [R006](https
Count: 0
###  [R007](https
Count: 0
###  [R008](https
Count: 0
###  [R009](https
Count: 0
###  [R010](https
Count: 64
[List matches](./results/R010.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_codedeploy_deployment_group.go:684:3: R010: prefer d.Get() over d.GetChange() when only using second return value`

###  [R011](https
Count: 0
###  [R012](https
Count: 0
###  [R013](https
Count: 0
###  [R014](https
Count: 0
###  [S001](https
Count: 0
###  [S002](https
Count: 0
###  [S003](https
Count: 0
###  [S004](https
Count: 0
###  [S005](https
Count: 0
###  [S006](https
Count: 0
###  [S007](https
Count: 0
###  [S008](https
Count: 0
###  [S009](https
Count: 0
###  [S010](https
Count: 0
###  [S011](https
Count: 0
###  [S012](https
Count: 0
###  [S013](https
Count: 0
###  [S014](https
Count: 0
###  [S015](https
Count: 0
###  [S016](https
Count: 0
###  [S017](https
Count: 0
###  [S018](https
Count: 0
###  [S019](https
Count: 0
###  [S020](https
Count: 0
###  [S021](https
Count: 0
###  [S022](https
Count: 0
###  [S023](https
Count: 0
###  [S024](https
Count: 0
###  [S025](https
Count: 0
###  [S026](https
Count: 0
###  [S027](https
Count: 0
###  [S028](https
Count: 0
###  [S029](https
Count: 0
###  [S030](https
Count: 0
###  [S031](https
Count: 0
###  [S032](https
Count: 0
###  [S033](https
Count: 0
###  [S034](https
Count: 0
###  [S035](https
Count: 0
###  [S036](https
Count: 0
###  [S037](https
Count: 0
###  [V001](https
Count: 126
[List matches](./results/V001.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/validators.go:2281:1: V001: custom SchemaValidateFunc should be replaced with validation.StringMatch() or validation.StringDoesNotMatch()`

###  [V002](https
Count: 0
###  [V003](https
Count: 0
###  [V004](https
Count: 0
###  [V005](https
Count: 0
###  [V006](https
Count: 0
###  [V007](https
Count: 0
###  [V008](https
Count: 0
