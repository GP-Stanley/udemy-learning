# map-data-type.tf (Base Code)

```bash
variable "my-map" {
  type = map
}

output "variable_value" {
  value = var.my-map
}
```

# map-data-type.tf (Final Code)

```bash
variable "my-map" {
  type = map
  default = {
    Name = "Alice"
    Team = "Payments"
  }
}

output "variable_value" {
  value = var.my-map
}
```