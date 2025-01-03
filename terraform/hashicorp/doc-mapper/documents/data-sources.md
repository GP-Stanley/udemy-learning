# Documentation Referred:
* https://registry.terraform.io/providers/digitalocean/digitalocean/latest/docs/data-sources/account
* https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/instance
* https://registry.terraform.io/providers/hashicorp/local/latest/docs/data-sources/file

# Code Used In Video:

## data-source-01.tf

```bash
terraform {
  required_providers {
    digitalocean = {
      source  = "digitalocean/digitalocean"
    }
  }
}


provider "digitalocean" {
  token = "your-token-here"
}

data "digitalocean_account" "example" {}
```

## data-source-02.tf

```bash
data "local_file" "foo" {
  filename = "${path.module}/demo.txt"
}
output "data" {
    value = data.local_file.foo.content
}
```

## data-source-03.tf

```bash
provider "aws" {
    region = "us-east-1"
}

data "aws_instances" "example" {}
```

<br>

# Data Sources Format

## Documentation Referred:
* https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/instance

## data-source-format.tf

```bash
provider "aws" {
    region = "us-east-1"
}

data "aws_instance" "example" {
 filter {
    name   = "tag:Team"
    values = ["Production"]
  }
}
```