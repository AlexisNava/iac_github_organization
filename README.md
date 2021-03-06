# iac_github_organization

Infrastructure as Code for a GitHub organization.

[TerraformOrgTest](https://github.com/TerraformOrgTest) is an example of the output of this project. 

## Requirements

- [Terraform >= v0.12.28](https://www.terraform.io/downloads.html)
- [GitHub Token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token) with the following permissions:
  - admin:org
  - admin:public_key
  - delete_repo
  - repo
  - user 

## Installation

### Initialize the project

```sh
terraform init
```

### Install the local modules

```sh
terraform get
```

## Module Documentation

- [github_repository](./modules/github_repository/README.md)

## Inputs

| Name           | Description       | Type   | Default | Required |
| :---:          | :---:             | :---:  | :---:   | :---:    |
| github_token | GitHub with the access to apply all the terraform configuration of the project | string | -       | :heavy_check_mark: |

## License

**iac_github_organization** is licensed under [Apache License, Version 2.0](./LICENSE).