# This snippet is from the Debugging Terraform video.

```bash
export TF_LOG_PATH=/tmp/crash.log
export TF_LOG=TRACE
```

# Base Code Used (tf-logs.tf)

```bash
resource "local_file" "foo" {
  content  = "foo!"
  filename = "${path.module}/foo.txt"
}
```

# Set ENV Variable in Windows

```bash
set TF_LOG=INFO
set TF_LOG=TRACE

set TF_LOG_PATH=terraform.txt
```

# Set ENV Variable in Linux / macOS

```bash
export TF_LOG=INFO
export TF_LOG=TRACE

export TF_LOG_PATH=terraform.txt
```