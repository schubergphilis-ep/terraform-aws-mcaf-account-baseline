# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [7.1.2](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v7.1.1...v7.1.2) (2026-07-07)


### 🐛 Fixes

* migrate MCAF module sources ([#2](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/issues/2)) ([c1da4ba](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/c1da4ba6bc38bacc021b6c2f2d8c0276a22702a6))

## [7.1.1](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v7.1.0...v7.1.1) (2026-07-01)


### 🐛 Fixes

* Skip EBS snapshot public access block resource when state is unblocked ([#34](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/34)) ([24d1fbe](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/24d1fbeb3255be2eaeaa535dd827b913637acc57))

## [7.1.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v7.0.1...v7.1.0) (2025-12-22)


### 🚀 Features

* require unmanaged ebs BPA with declarative policies ([#32](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/32)) ([dd842ca](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/dd842ca6eb1a493cbda40d3cce850e9ce8a8df6b))

## [7.0.1](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v7.0.0...v7.0.1) (2025-10-31)


### 🐛 Fixes

* bug: solve known after apply issue with the aws_ebs_default_kms_key resource ([#30](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/30)) ([535a6cd](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/535a6cdb5c0664d04f8bd58a311f05729184b1a3))

## [7.0.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v6.1.0...v7.0.0) (2025-10-31)


### ⚠ BREAKING CHANGES

* switch to per-region KMS keys to enable multi-region EBS default encryption and optionally ssm automation log group encryption ([#29](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/29))

### 🚀 Features

* switch to per-region KMS keys to enable multi-region EBS default encryption and optionally ssm automation log group encryption ([#29](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/29)) ([a4ab430](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/a4ab4309407fb6785e0ad88956f8d8e4c8ec03b1))

## [6.1.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v6.0.0...v6.1.0) (2025-10-28)


### 🚀 Features

* Push SSM automation logging to cloudwatch logs by default to solve Security Hub SSM.6 finding. ([#28](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/28)) ([60807dd](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/60807dddc2130c1eebd68d03d13be06e8f261f0d))

## [6.0.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v5.0.1...v6.0.0) (2025-10-28)


### ⚠ BREAKING CHANGES

* align variable naming with mcaf-landing-zone and solve deprecation warnings ([#27](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/27))

### 🚀 Features

* align variable naming with mcaf-landing-zone and solve deprecation warnings ([#27](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/27)) ([825c8e3](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/825c8e34821a4e9793593eaa5ad0b816e49ae987))

## [5.0.1](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v5.0.0...v5.0.1) (2025-10-20)


### 🐛 Fixes

* ensure regions to baseline is an distinct list of values ([#26](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/26)) ([8f6f281](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/8f6f2818b4f8107855fc15ad377ed299b796d7c7))

## [5.0.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v4.0.0...v5.0.0) (2025-08-12)


### 🚀 Features

* breaking: multi region support ([#25](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/25)) ([a4f23e7](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/a4f23e76c9820305b0d90c04d0d2d9e4e2939770))

## [4.0.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v3.0.0...v4.0.0) (2025-06-20)


### 🚀 Features

* breaking: add enable_additional_eu_regions variable ([#23](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/23)) ([a151b12](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/a151b123db907a8e31f448f80c2a13ce455d64b9))

## [3.0.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v2.0.1...v3.0.0) (2025-05-21)


### 🚀 Features

* breaking: block public EC2 artifacts shares by default ([#22](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/22)) ([f49ad28](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/f49ad28cc7348f40b3d4552573c91db5b010a65f))

## [2.0.1](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v2.0.0...v2.0.1) (2025-02-19)

## [2.0.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v1.1.0...v2.0.0) (2025-01-16)


### 🚀 Features

* breaking: remove aws_security_hub_standards_arns to support centralized security hub configuration ([#19](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/19)) ([27058ad](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/27058ad459d33af7da8f2c38605319fca5eae37d))

## [1.1.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v1.0.1...v1.1.0) (2025-01-14)


### 🚀 Features

* allow to configure the aws s3 account public access block ([#18](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/18)) ([3276bc1](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/3276bc11a53d52cc30e9252446259bffdc77bd85))

## [1.0.1](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v1.0.0...v1.0.1) (2024-01-02)

## [1.0.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.3.1...v1.0.0) (2024-01-02)


### 🚀 Features

* breaking: Control Tower 3.0 support ([#15](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/15)) ([24a516c](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/24a516c62dfcc8e7c93f901f1c5124be919b0cca))

## [0.3.1](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.3.0...v0.3.1) (2024-01-02)


### 🐛 Fixes

* bug: modify service quotas manager role name ([#16](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/16)) ([b745859](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/b745859c30c5444e593e7fee27e445033ae4d354))

## [0.3.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.2.1...v0.3.0) (2023-12-28)


### 🚀 Features

* add role to integrate with the terraform-aws-mcaf-service-quotas-manager module + formatting ([#14](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/14)) ([c036e2d](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/c036e2d2df6937903e4749538c64a699ae14c596))

## [0.2.1](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.2.0...v0.2.1) (2023-12-05)


### 🐛 Fixes

* bug: Fix `aws_cloudwatch_log_group` resource ([#13](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/13)) ([348ccd6](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/348ccd69015cdf464a752ffcbf24c03c30bdd70e))

## [0.2.0](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.1.5...v0.2.0) (2023-07-25)


### 🚀 Features

* control the AWS Security Hub standards in member accounts ([#12](https://github.com/schubergphilis/terraform-aws-mcaf-account-baseline/pull/12)) ([7ba5c65](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/commit/7ba5c65ca2442fe0e53881caa0c8032ed068904c))

## [0.1.5](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.1.4...v0.1.5) (2023-05-01)

## [0.1.4](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.1.3...v0.1.4) (2023-04-03)

## [0.1.3](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.1.2...v0.1.3) (2021-09-09)

## [0.1.2](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.1.1...v0.1.2) (2021-06-04)

## [0.1.1](https://github.com/schubergphilis-ep/terraform-aws-mcaf-account-baseline/compare/v0.1.0...v0.1.1) (2021-05-21)

## 0.1.0 (2021-02-26)
