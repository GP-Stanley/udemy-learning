# Exam Preparation Practice Test - 2

1. Following is an exert of the code which Alice has written. There is a reference to count.index in Tags.

```bash
variable "tags" {
  type = list
  default = ["firstec2","secondec2","thirdec2"]
}
 
  tags = {
     Name = element(var.tags,count.index)
   }
```

**If count.index is set to 1, which of the following values will be used?**

Answer:
   * secondec2
   * count.index counts the distinct index number (starting with 0)

<br>

<hr style="height:4px;background:grey">

<br>

2. Alice is writing a module, and within the module, there are multiple places where she has defined the same set of Terraform expression.

    Whenever there is modification required in the expression, Alice has to go through multiple places in the code and modify everywhere.

    **What is a better approach to dealing with this?**

Answer:
* Use local values to define the repeated Terraform expression in one place and reference it throughout the module. This approach simplifies maintenance and ensures consistency.
* *Documentation*: https://www.terraform.io/language/values/locals

<br>

<hr style="height:4px;background:grey">

<br>

3. Enterprise Corp has a Terraform State file that contains details related to 100s of resources that are currently created in their Cloud Infrastructure.

    There is a requirement to quickly list all the resources that are part of the state file.

    **What is the best way to achieve this?**

Answer:
* terraform state list
* This command will list all of the resources in the state file, sorted by module depth order followed by alphabetical order. 
* *Documentation*: https://www.terraform.io/cli/commands/state/list

<br>

<hr style="height:4px;background:grey">

<br>

4. Matthew has created an EC2 instance via Terraform. Matthew has defined the following rules within the security group:
   * `Port 443 allowed from 0.0.0.0/0`
   * `Port 22 allowed from 125.36.50.23/32`

    John has added the following rule manually:
    * `Port 80 allowed from 0.0.0.0/0`

    **Next time when Matthew runs a terraform plan, what will happen?**

Answer:
* Terraform plan will show output to remove the manually created rule.

<br>

<hr style="height:4px;background:grey">

<br>

5. Medium Corp is using the Terraform Workspace feature.

    After the "terraform apply" is completed, the terraform.tfstate file does not appear in the main project directory.

    **In which directory is the terraform.tfstate file created?**

Answer:
* terraform.tfstate.d
* *Documentation*: https://www.terraform.io/language/state/workspaces

<br>

<hr style="height:4px;background:grey">

<br>

6. Yes or no. James has decided not to use the terraform.tfvars file, instead, he wants to store all data in custom.tfvars file. **Is it possible?**

Answer:
* Yes.
* This will work however user will have to explicitly specify the tfvars file during the apply operation. 
* *Sample command*: terraform apply -var-file="custom.tfvars"

<br>

<hr style="height:4px;background:grey">

<br>

7. Where do we define provisioner block in Terraform?

```bash
resource "aws_instance" "myec2" {
  ami           = "ami-082b5a644766e0e6f"
  instance_type = "t2.micro"
}
```

Answer:
* Inside the resource group.
* *Documentaiton*: https://www.terraform.io/language/resources/provisioners/syntax

<br>

<hr style="height:4px;background:grey">

<br>

8. True or false. Following is the sample Child module configuration:

```bash
resource "aws_instance" "myec2" {
  ami           = "ami-082b5a644766e0e6f"
  instance_type = var.instance_type
}

variable instance_type {}
```

**If this module is called from a ROOT module, can the user set the value associated with variable of instance_type?**

Answer:
* True. 
* If this module is called from a root module, the user can set the value associated with the instance_type variable. 
* The root module can pass the value to the child module by defining the variable in the module block.

<br>

<hr style="height:4px;background:grey">

<br>

9. Yes or no. Matthew has referred to a child module that has the following code. 

```bash
resource "aws_instance" "myec2" {
   ami = "ami-082b5a644766e0e6f"
   instance_type = "t2.micro
}
```

**Can Matthew override the instance_type from t2.micro to t2.large from the ROOT module directly?**

Answer:
* No. 
* Matthew cannot override the instance_type from t2.micro to t2.large directly from the root module because the instance_type is hardcoded in the child module.

<br>

<hr style="height:4px;background:grey">

<br>

10. Based on the following lookup function example, what data type is referenced?

`    lookup({a="ay", b="bee"}, "a", "what?")`

Answer:
* Map.
* *Documentation*: https://www.terraform.io/language/functions/lookup

<br>

<hr style="height:4px;background:grey">

<br>

11. James has decided to not use the terraform.tfvars file, instead, he wants to store all data into custom.tfvars file?  

    **How can he deal with this use-case while running terraform plan?**

Answer:
* terraform plan -var-file="custom.tfvars"
* *Documentation*: https://www.terraform.io/language/values/variables#variable-definitions-tfvars-files

<br>

<hr style="height:4px;background:grey">

<br>

12. Yes or no. John is an intern, and he had recently created an EC2 instance manually.

    **Can he import the EC2 instance to Terraform without having to write a Terraform configuration file for that EC2 instance from scratch?**

Answer:
* Yes.
* He can use the terraform import command to bring the existing resource under Terraform management. 
* After importing, he can run terraform plan to see the current state and make any necessary adjustments to the configuration file.
* *Documentation*: https://developer.hashicorp.com/terraform/cli/import

<br>

<hr style="height:4px;background:grey">

<br>

13. Matthew has written the configuration file of a manually created EC2 instance in Terraform. Following is the code:

```bash
resource "aws_instance" "myec2" {
  ami = "ami-bf5540df"
  instance_type = "t2.micro"
  vpc_security_group_ids = ["sg-6ae7d613", "sg-53370035"]
  key_name = "remotepractical"
  subnet_id = "subnet-9e3cfbc5"
 
  tags {
    Name = "manual"
  }
}
```

The instance id of the manually created EC2 instance is `i-041886ebb7e9bd20` **How he can import data of that EC2 to the state file and link it with the resource block?**

Answer:
* terraform import aws_instance.myec2 i-041886ebb7e9bd20
* *Documentation*: https://www.terraform.io/cli/import/usage

<br>

<hr style="height:4px;background:grey">

<br>

14. John is working as a DevOps Engineer and is managing the Terraform Infrastructure.

    Based on a new requirement, John has to create a new security group (firewall), and 60 different ports need to be whitelisted in this firewall.

    John wants to avoid writing 60 different ingress blocks and maintain (add/remove) whenever a new IP address needs to be added or removed in the subsequent updates.

```bash
  ingress {
    description      = "kplabs-sg"
    from_port        = 443
    to_port          = 443
    protocol         = "tcp"
    cidr_blocks      = 172.31.0.5
  }
```

**Which Terraform functionality can John use to minimize the overall Terraform code that can also be managed easily?**

Answer:
* Dynamic blocks.
* John can use dynamic blocks in Terraform to minimize the overall code and manage it easily. 
* Dynamic blocks allow you to generate multiple nested blocks within a resource based on a list or map.
* Dynamic blocks allow you to generate a collection of resources based on a list of values. 
* This is useful for creating repetitive resources, such as security group rules. 
* *Documentation*: https://www.terraform.io/language/expressions/dynamic-blocks

<br>

<hr style="height:4px;background:grey">

<br>

15. Alice has added a simple variable definition in Terraform code.

```bash
variable "kpnumber" { 
default = 3
}
```

Alice also has defined the following environment variable: `TF_kpnumber=6`, `TF_VAR_kpnumber=9`.

There is also a `terraform.tfvars` file with the following contents

`kpnumber = 7`

**When you run the following apply command, what is the value assigned to the number variable?**

`terraform apply -var kpnumber=4`

Answer:
* 4.
  * This is because the -var option provided in the command line has the highest precedence over other methods of setting variable values, such as environment variables, .tfvars files, and default values.
* command-line argument "-var kpnumber=4" has the highest precedence, so the value of the kpnumber variable will be set to 4, other values that defined for the kpnumber variable will be ignored. 
* *Documentation*: https://www.terraform.io/language/values/variables#variable-definition-precedence

<br>

<hr style="height:4px;background:grey">

<br>

16. True or false. Matthew is trying to achieve a use-case that is not directly supported by default Terraform functions that are available.

    **Can Matthew create his own set of function that his team can use for custom use-cases?**

Answer:
* False.
* The Terraform language does not support user-defined functions, and so only the functions built in to the language are available for use

<br>

<hr style="height:4px;background:grey">

<br>

17. True or false. Matthew has created a new workspace named "DEV".

    **Does Matthew needs to manually switch to the DEV workspace in order to start using it?**

Answer:
* False.
* By default, when you create a new workspace you are automatically switched to it.

<br>

<hr style="height:4px;background:grey">

<br>

18. **Are there any different ways to destroy the resources without needing to run terraform destroy command?**

Answer:
* Yes.
*  You can also simply remove the resource configuration from your code and run Terraform apply. 
*  This will also destroy the resource.

<br>

<hr style="height:4px;background:grey">

<br>

19. **If a user directly runs terraform apply without running the terraform plan, will the apply operation fail?**

Answer:
* No.
* When you run terraform apply without passing a saved plan file, Terraform automatically creates a new execution plan as if you had run terraform plan, prompts you to approve that plan, and takes the indicated actions.

<br>

<hr style="height:4px;background:grey">

<br>

20. Due to some issues, the state file is in a locked state, and users are not able to perform terraform apply operations further.

    **What actions can be taken to overcome this?**

Answer:
* You can use the terraform force-unlock command to manually unlock the state file. 
* This command is useful when the state file remains locked due to a process not releasing it properly, such as a terminated session or a network issue.
* "terraform force-unlock" command can be used to unlock a Terraform state file that is locked by another process. 
* *Documentation*: https://www.terraform.io/docs/commands/force-unlock.html

<br>

<hr style="height:4px;background:grey">

<br>

21. **Do all the backends that are supported in Terraform has the state locking functionality?**

Answer:
* No.  

<br>

<hr style="height:4px;background:grey">

<br>

22. **Does terraform refresh perform any kind of modification on the running infrastructure?**

Answer:
* No. 
* The terraform refresh command reads the current settings from all managed remote objects and updates the Terraform state to match.

<br>

<hr style="height:4px;background:grey">

<br>

23. James needs to make use of the module within his terraform code.

    **Should the module always need to  be public and open-source to be able to be used?**

Answer:
* No. 

<br>

<hr style="height:4px;background:grey">

<br>

24. Matthew is writing a module and within the module, there are multiple places where he has to use the same conditional expression but he wants to avoid repeating the same values or expressions multiple times in a configuration.

    **What is a better approach to dealing with this?**

Answer:
* Local values.

<br>

<hr style="height:4px;background:grey">

<br>

25. A variable named demo has following value. What is the data type of the variable?

    `demo = ["admin","alice"]`

Answer:
* List.
* List represents a sequence of values, like ["us-west-1a", "us-west-1c"].

<br>

<hr style="height:4px;background:grey">

<br>

26. **What does the following data represents in Terraform?**

    * max
    * min
    * element
    * join
    * concat
    * file

Answer:
* Functions.

<br>

<hr style="height:4px;background:grey">

<br>

27. Matthew works as a DevOps Engineer in Enterprise Corp.

    Whenever he runs operations like terraform plan, terraform apply, it takes a lot of time.

    **What can be the issue behind this?**

Answer:
* Terraform performs sync for all resources in the state file by default for every plan and apply. 
* If there are a lot of resources, it can slow down the operation.

<br>

<hr style="height:4px;background:grey">

<br>

28. **If there is any disperency between the current and desired state of the infrastructure, can terraform validate command display the issue?**

Answer:
* No.
* The terraform validate command validates the configuration files in a directory, referring only to the configuration and not accessing any remote services such as remote state, provider APIs, etc.

<br>

<hr style="height:4px;background:grey">

<br>

29. Following are the output values defined in Child and Root Module:

Child Module
```bash
output "child_module" {
  value = "This is Child Module"
}
```
Root Module:
```bash
output "root_module" {
  value = "This is ROOT Module"
}
```

**On a terraform apply, which output values will be displayed?**

Answer:
* When you run terraform apply, only the output values from the root module will be displayed. 
* The output values from the child module will not be displayed directly unless they are explicitly referenced in the root module's output.

<br>

<hr style="height:4px;background:grey">

<br>

30. Alice has started to make use of Terraform Cloud Workspace and has linked a Git Repository to it.

    **Whenever a new code change is committed to the version control repository, will Terraform automatically run the terraform plan operation?**

Answer:
* True.
* Terraform Cloud will automatically run a terraform plan operation whenever a new code change is committed to the version control repository that is linked to the workspace.

<br>

<hr style="height:4px;background:grey">

<br>

31. A variable name "update" must only support boolean value.

    **How can we define the type of value that is expected for a specific variable?**

Answer:
* Use type in variable block.

For example:
```bash
variable "update" {
  type    = bool
  default = false
}
```

<br>

<hr style="height:4px;background:grey">

<br>

32. **Which among the following allows constructing a set of nested configuration blocks?** if else statement, for_each, resource, dynamic blocks

Answer:
* dynamic blocks allow constructing a set of nested configuration blocks in Terraform. 
* Dynamic blocks enable you to generate multiple nested blocks within a resource based on a list or map, making it easier to manage and maintain complex configurations.

<br>

<hr style="height:4px;background:grey">

<br>

