<!-- This file was automatically generated by the `build-harness`. Make all changes to `README.yaml` and run `make readme` to rebuild this file. -->

[![Cloud Posse](https://cloudposse.com/logo-300x69.svg)](https://cloudposse.com)

# terraform-aws-ec2-bastion-server [![Build Status](https://travis-ci.org/cloudposse/terraform-aws-ec2-bastion-server.svg?branch=master)](https://travis-ci.org/cloudposse/terraform-aws-ec2-bastion-server) [![Latest Release](https://img.shields.io/github/release/cloudposse/terraform-aws-ec2-bastion-server.svg)](https://github.com/cloudposse/terraform-aws-ec2-bastion-server/releases/latest) [![Slack Community](https://slack.cloudposse.com/badge.svg)](https://slack.cloudposse.com)


Terraform module to define a generic Bastion host with parameterized `user_data`


---

This project is part of our comprehensive ["SweetOps"](https://docs.cloudposse.com) approach towards DevOps. 


It's 100% Open Source and licensed under the [APACHE2](LICENSE).











## Makefile Targets
```
Available targets:

  help                                This help screen
  help/all                            Display help for all targets
  lint                                Lint terraform code

```

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| ami | the AMI to use | string | `ami-efd0428f` | no |
| instance_type | Elastic cache instance type | string | `t2.micro` | no |
| key_name | Key name | string | `` | no |
| name | The Name of the application or solution  (e.g. `bastion` or `portal`) | string | `bastion` | no |
| namespace | Namespace (e.g. `cp` or `cloudposse`) | string | `global` | no |
| security_groups | AWS security group ids | list | - | yes |
| ssh_user | Default SSH user for this AMI. e.g. `ec2user` for Amazon Linux and `ubuntu` for Ubuntu systems | string | `ec2user  `or`  ubuntu` | no |
| stage | Stage (e.g. `prod`, `dev`, `staging`) | string | `default` | no |
| subnets | AWS subnet ids | list | `<list>` | no |
| user_data | User data scripts content | list | `<list>` | no |
| user_data_file | User data file | string | `user_data.sh` | no |
| vpc_id | VPC ID | string | `` | no |
| zone_id | Route53 DNS Zone id | string | `` | no |

## Outputs

| Name | Description |
|------|-------------|
| instance_id | Instance id |
| private_ip | Private IP of instance |
| public_ip | Public IP of instance (or EIP) |
| role | Name of AWS IAM Role associated with the instance |
| security_group_id | Security group id |
| ssh_user | SSH user |




## Related Projects

Check out these related projects.

- [bastion](https://github.com/cloudposse/bastion) - 🔒Secure Bastion implemented as Docker Container running Alpine Linux with Google Authenticator & DUO MFA support
- [terraform-aws-ec2-instance](https://github.com/cloudposse/terraform-aws-ec2-instance) - Terraform Module for providing a general EC2 instance provisioned by Ansible
- [terraform-aws-ec2-ami-backup](https://github.com/cloudposse/terraform-aws-ec2-ami-backup) - Terraform module for automatic & scheduled AMI creation



## Help

**Got a question?**

File a GitHub [issue](https://github.com/cloudposse/terraform-aws-ec2-bastion-server/issues), send us an [email][email] or join our [Slack Community][slack].

## Commerical Support

Work directly with our team of DevOps experts via email, slack, and video conferencing. 

We provide *commercial support* for all of our [Open Source][github] projects. As a *Dedicated Support* customer, you have access to our team of subject matter experts at a fraction of the cost of a fulltime engineer. 

[![E-Mail](https://img.shields.io/badge/email-hello@cloudposse.com-blue.svg)](mailto:hello@cloudposse.com)

- **Questions.** We'll use a Shared Slack channel between your team and ours.
- **Troubleshooting.** We'll help you triage why things aren't working.
- **Code Reviews.** We'll review your Pull Requests and provide constructive feedback.
- **Bug Fixes.** We'll rapidly work to fix any bugs in our projects.
- **Build New Terraform Modules.** We'll develop original modules to provision infrastructure.
- **Cloud Architecture.** We'll assist with your cloud strategy and design.
- **Implementation.** We'll provide hands on support to implement our reference architectures. 


## Community Forum

Get access to our [Open Source Community Forum][slack] on Slack. It's **FREE** to join for everyone! Our "SweetOps" community is where you get to talk with others who share a similar vision for how to rollout and manage infrastructure. This is the best place to talk shop, ask questions, solicit feedback, and work together as a community to build *sweet* infrastructure.

## Contributing

### Bug Reports & Feature Requests

Please use the [issue tracker](https://github.com/cloudposse/terraform-aws-ec2-bastion-server/issues) to report any bugs or file feature requests.

### Developing

If you are interested in being a contributor and want to get involved in developing this project or [help out](https://github.com/orgs/cloudposse/projects/3) with our other projects, we would love to hear from you! Shoot us an [email](mailto:hello@cloudposse.com).

In general, PRs are welcome. We follow the typical "fork-and-pull" Git workflow.

 1. **Fork** the repo on GitHub
 2. **Clone** the project to your own machine
 3. **Commit** changes to your own branch
 4. **Push** your work back up to your fork
 5. Submit a **Pull Request** so that we can review your changes

**NOTE:** Be sure to merge the latest changes from "upstream" before making a pull request!


## Copyright

Copyright © 2017-2018 [Cloud Posse, LLC](https://cloudposse.com)



## License 

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) 

See [LICENSE](LICENSE) for full details.

    Licensed to the Apache Software Foundation (ASF) under one
    or more contributor license agreements.  See the NOTICE file
    distributed with this work for additional information
    regarding copyright ownership.  The ASF licenses this file
    to you under the Apache License, Version 2.0 (the
    "License"); you may not use this file except in compliance
    with the License.  You may obtain a copy of the License at

      https://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing,
    software distributed under the License is distributed on an
    "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.


## Trademarks

All other trademarks referenced herein are the property of their respective owners.

## About

This project is maintained and funded by [Cloud Posse, LLC][website]. Like it? Please let us know at <hello@cloudposse.com>

[![Cloud Posse](https://cloudposse.com/logo-300x69.svg)](https://cloudposse.com)

We're a [DevOps Professional Services][hire] company based in Los Angeles, CA. We love [Open Source Software](https://github.com/cloudposse/)!

We offer paid support on all of our projects.  

Check out [our other projects][github], [apply for a job][jobs], or [hire us][hire] to help with your cloud strategy and implementation.

  [docs]: https://docs.cloudposse.com/
  [website]: https://cloudposse.com/
  [github]: https://github.com/cloudposse/
  [jobs]: https://cloudposse.com/jobs/
  [hire]: https://cloudposse.com/contact/
  [slack]: https://slack.cloudposse.com/
  [linkedin]: https://www.linkedin.com/company/cloudposse
  [twitter]: https://twitter.com/cloudposse/
  [email]: mailto:hello@cloudposse.com


### Contributors

|  [![Andriy Knysh][aknysh_avatar]][aknysh_homepage]<br/>[Andriy Knysh][aknysh_homepage] | [![Igor Rodionov][goruha_avatar]][goruha_homepage]<br/>[Igor Rodionov][goruha_homepage] | [![Bobby Larson][karma0_avatar]][karma0_homepage]<br/>[Bobby Larson][karma0_homepage] |
|---|---|---|

  [aknysh_homepage]: https://github.com/aknysh
  [aknysh_avatar]: https://github.com/aknysh.png?size=150
  [goruha_homepage]: https://github.com/goruha
  [goruha_avatar]: https://github.com/goruha.png?size=150
  [karma0_homepage]: https://github.com/karma0
  [karma0_avatar]: https://github.com/karma0.png?size=150


