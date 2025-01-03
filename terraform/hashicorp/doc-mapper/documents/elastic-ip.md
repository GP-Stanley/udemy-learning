Documentation Referred: https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/eip

# eip.tf

```bash
resource "aws_eip" "lb" {
  domain   = "vpc"
}
```

## Commands Used:

```bash
terraform apply -auto-approve
terraform destroy -auto-approve
```