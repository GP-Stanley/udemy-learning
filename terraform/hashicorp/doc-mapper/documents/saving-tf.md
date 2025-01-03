# This snippet is from the "Savings Terraform Plan To File" video.

## local_file.tf

```bash
resource "local_file" "foo" {
  content  = "Hello World"
  filename = "terraform.txt"
}
```

## Commands Used:

```bash
terraform plan -out=infra.plan
terraform apply infra.plan
```

```bash
terraform show infra.plan
terraform show -json infra.plan
```

```bash
terraform show -json infra.plan | jq
```