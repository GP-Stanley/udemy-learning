# ec2.tf

```bash
resource "aws_instance" "myec2" {
   ami = "ami-082b5a644766e0e6f"
   instance_type = "t2.micro"
}

resource "aws_instance" "newec2" {
   ami = "ami-082b5a644766e0e6f"
   instance_type = "t2.micro"
}
```

# iam_user.tf

```bash
resource "aws_iam_user" "lb" {
  name = var.iam_user
  path = "/system/"
}
```

# provider.tf

```bash
provider "aws" {
  region     = "us-west-2"
  access_key = "YOUR-ACCESS-KEY"
  secret_key = "YOUR-SECRET-KEY"
}
```

# semantics.tf

```bash
provider "aws" {
  region     = "us-west-2"
  access_key = "YOUR-ACCESS-KEY"
  secret_key = "YOUR-SECRET-KEY"
}

variable "iam_user" {
  default = "demouser"
}

resource "aws_instance" "myec2" {
   ami = "ami-082b5a644766e0e6f"
   instance_type = "t2.micro"
}

resource "aws_iam_user" "lb" {
  name = var.iam_user
  path = "/system/"
}
```

# variables.tf

```bash
variable "iam_user" {
  default = "demouser"
}
```