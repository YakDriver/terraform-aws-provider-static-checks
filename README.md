![Travis CI Status](https://travis-ci.org/YakDriver/terraform-aws-provider-static-checks.svg?branch=main)
# terraform-aws-provider-static-checks

Automatic daily rebuilds! This repo shows the current state of static checks in the Terraform AWS provider Go code. This repo uses the [awsproviderlint](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint) and [tfproviderlint](https://github.com/bflad/tfproviderlint).

# Checks
## awsproviderlint

###  [AWSAT001](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint/passes/AWSAT001)
Count: 0
###  [AWSAT002](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint/passes/AWSAT002)
Count: 24
[List matches](./results/AWSAT002.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_instance_test.go:3513:52: AWSAT002: AMI IDs should not be hardcoded`

###  [AWSAT003](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint/passes/AWSAT003)
Count: 720
[List matches](./results/AWSAT003.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_ec2_transit_gateway_vpc_attachment_test.go:825:21: AWSAT003: regions should not be hardcoded, use aws_region and aws_availability_zones data sources instead`

###  [AWSAT004](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint/passes/AWSAT004)
Count: 0
###  [AWSAT005](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint/passes/AWSAT005)
Count: 228
[List matches](./results/AWSAT005.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_ssm_resource_data_sync_test.go:149:21: AWSAT005: avoid hardcoded ARN AWS partitions, use aws_partition data source`

###  [AWSAT006](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint/passes/AWSAT006)
Count: 506
[List matches](./results/AWSAT006.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_emr_cluster_test.go:3086:21: AWSAT006: avoid hardcoding AWS partition DNS suffixes, instead use the aws_partition data source`

###  [AWSR001](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint/passes/AWSR001)
Count: 0
###  [AWSR002](https://github.com/terraform-providers/terraform-provider-aws/tree/master/awsproviderlint/passes/AWSR002)
Count: 0
## tfproviderlint

###  [AT001](https://github.com/bflad/tfproviderlint/tree/master/passes/AT001)
Count: 0
###  [AT002](https://github.com/bflad/tfproviderlint/tree/master/passes/AT002)
Count: 0
###  [AT003](https://github.com/bflad/tfproviderlint/tree/master/passes/AT003)
Count: 0
###  [AT004](https://github.com/bflad/tfproviderlint/tree/master/passes/AT004)
Count: 15
[List matches](./results/AT004.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_instance_test.go:3835:46: AT004: provider declaration should be omitted`

###  [AT005](https://github.com/bflad/tfproviderlint/tree/master/passes/AT005)
Count: 0
###  [AT006](https://github.com/bflad/tfproviderlint/tree/master/passes/AT006)
Count: 0
###  [AT007](https://github.com/bflad/tfproviderlint/tree/master/passes/AT007)
Count: 0
###  [AT008](https://github.com/bflad/tfproviderlint/tree/master/passes/AT008)
Count: 0
###  [R001](https://github.com/bflad/tfproviderlint/tree/master/passes/R001)
Count: 17
[List matches](./results/R001.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_sns_sms_preferences.go:137:9: R001: ResourceData.Set() key argument should be string literal`

###  [R002](https://github.com/bflad/tfproviderlint/tree/master/passes/R002)
Count: 0
###  [R003](https://github.com/bflad/tfproviderlint/tree/master/passes/R003)
Count: 0
###  [R004](https://github.com/bflad/tfproviderlint/tree/master/passes/R004)
Count: 0
###  [R005](https://github.com/bflad/tfproviderlint/tree/master/passes/R005)
Count: 0
###  [R006](https://github.com/bflad/tfproviderlint/tree/master/passes/R006)
Count: 0
###  [R007](https://github.com/bflad/tfproviderlint/tree/master/passes/R007)
Count: 0
###  [R008](https://github.com/bflad/tfproviderlint/tree/master/passes/R008)
Count: 0
###  [R009](https://github.com/bflad/tfproviderlint/tree/master/passes/R009)
Count: 0
###  [R010](https://github.com/bflad/tfproviderlint/tree/master/passes/R010)
Count: 64
[List matches](./results/R010.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/resource_aws_sns_topic.go:251:3: R010: prefer d.Get() over d.GetChange() when only using second return value`

###  [R011](https://github.com/bflad/tfproviderlint/tree/master/passes/R011)
Count: 0
###  [R012](https://github.com/bflad/tfproviderlint/tree/master/passes/R012)
Count: 0
###  [R013](https://github.com/bflad/tfproviderlint/tree/master/passes/R013)
Count: 0
###  [R014](https://github.com/bflad/tfproviderlint/tree/master/passes/R014)
Count: 0
###  [S001](https://github.com/bflad/tfproviderlint/tree/master/passes/S001)
Count: 0
###  [S002](https://github.com/bflad/tfproviderlint/tree/master/passes/S002)
Count: 0
###  [S003](https://github.com/bflad/tfproviderlint/tree/master/passes/S003)
Count: 0
###  [S004](https://github.com/bflad/tfproviderlint/tree/master/passes/S004)
Count: 0
###  [S005](https://github.com/bflad/tfproviderlint/tree/master/passes/S005)
Count: 0
###  [S006](https://github.com/bflad/tfproviderlint/tree/master/passes/S006)
Count: 0
###  [S007](https://github.com/bflad/tfproviderlint/tree/master/passes/S007)
Count: 0
###  [S008](https://github.com/bflad/tfproviderlint/tree/master/passes/S008)
Count: 0
###  [S009](https://github.com/bflad/tfproviderlint/tree/master/passes/S009)
Count: 0
###  [S010](https://github.com/bflad/tfproviderlint/tree/master/passes/S010)
Count: 0
###  [S011](https://github.com/bflad/tfproviderlint/tree/master/passes/S011)
Count: 0
###  [S012](https://github.com/bflad/tfproviderlint/tree/master/passes/S012)
Count: 0
###  [S013](https://github.com/bflad/tfproviderlint/tree/master/passes/S013)
Count: 0
###  [S014](https://github.com/bflad/tfproviderlint/tree/master/passes/S014)
Count: 0
###  [S015](https://github.com/bflad/tfproviderlint/tree/master/passes/S015)
Count: 0
###  [S016](https://github.com/bflad/tfproviderlint/tree/master/passes/S016)
Count: 0
###  [S017](https://github.com/bflad/tfproviderlint/tree/master/passes/S017)
Count: 0
###  [S018](https://github.com/bflad/tfproviderlint/tree/master/passes/S018)
Count: 0
###  [S019](https://github.com/bflad/tfproviderlint/tree/master/passes/S019)
Count: 0
###  [S020](https://github.com/bflad/tfproviderlint/tree/master/passes/S020)
Count: 0
###  [S021](https://github.com/bflad/tfproviderlint/tree/master/passes/S021)
Count: 0
###  [S022](https://github.com/bflad/tfproviderlint/tree/master/passes/S022)
Count: 0
###  [S023](https://github.com/bflad/tfproviderlint/tree/master/passes/S023)
Count: 0
###  [S024](https://github.com/bflad/tfproviderlint/tree/master/passes/S024)
Count: 0
###  [S025](https://github.com/bflad/tfproviderlint/tree/master/passes/S025)
Count: 0
###  [S026](https://github.com/bflad/tfproviderlint/tree/master/passes/S026)
Count: 0
###  [S027](https://github.com/bflad/tfproviderlint/tree/master/passes/S027)
Count: 0
###  [S028](https://github.com/bflad/tfproviderlint/tree/master/passes/S028)
Count: 0
###  [S029](https://github.com/bflad/tfproviderlint/tree/master/passes/S029)
Count: 0
###  [S030](https://github.com/bflad/tfproviderlint/tree/master/passes/S030)
Count: 0
###  [S031](https://github.com/bflad/tfproviderlint/tree/master/passes/S031)
Count: 0
###  [S032](https://github.com/bflad/tfproviderlint/tree/master/passes/S032)
Count: 0
###  [S033](https://github.com/bflad/tfproviderlint/tree/master/passes/S033)
Count: 0
###  [S034](https://github.com/bflad/tfproviderlint/tree/master/passes/S034)
Count: 0
###  [S035](https://github.com/bflad/tfproviderlint/tree/master/passes/S035)
Count: 0
###  [S036](https://github.com/bflad/tfproviderlint/tree/master/passes/S036)
Count: 0
###  [S037](https://github.com/bflad/tfproviderlint/tree/master/passes/S037)
Count: 0
###  [V001](https://github.com/bflad/tfproviderlint/tree/master/passes/V001)
Count: 126
[List matches](./results/V001.txt)

Example: `/home/travis/gopath/src/github.com/terraform-providers/terraform-provider-aws/aws/validators.go:1394:1: V001: custom SchemaValidateFunc should be replaced with validation.StringMatch() or validation.StringDoesNotMatch()`

###  [V002](https://github.com/bflad/tfproviderlint/tree/master/passes/V002)
Count: 0
###  [V003](https://github.com/bflad/tfproviderlint/tree/master/passes/V003)
Count: 0
###  [V004](https://github.com/bflad/tfproviderlint/tree/master/passes/V004)
Count: 0
###  [V005](https://github.com/bflad/tfproviderlint/tree/master/passes/V005)
Count: 0
###  [V006](https://github.com/bflad/tfproviderlint/tree/master/passes/V006)
Count: 0
###  [V007](https://github.com/bflad/tfproviderlint/tree/master/passes/V007)
Count: 0
###  [V008](https://github.com/bflad/tfproviderlint/tree/master/passes/V008)
Count: 0
