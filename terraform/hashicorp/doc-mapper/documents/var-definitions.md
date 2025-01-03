# Base Code

## variable-definition-file.tf

```bash
resource "aws_instance" "myec2" {
  ami           = "ami-0e670eb768a5fc3d4"
  instance_type = "t2.micro"
}
Final Code
variable-definition-file.tf
resource "aws_instance" "myec2" {
  ami           = var.ami
  instance_type = "t2.micro"
}
```

## variables.tf

```bash
variable "ami" {}
terraform.tfvars
ami = "ami-0e670eb768a5fc3d4"
```

## Commands Used in Video

```bash
terraform plan
terraform apply
terraform plan -var-file="prod.tfvars"
```