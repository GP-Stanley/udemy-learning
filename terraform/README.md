- [Terraform](#terraform)
  - [HashiCorp Certified: Terraform Associate 2024](#hashicorp-certified-terraform-associate-2024)
    - [HashiCorp Exam Preparation Practice Test](#hashicorp-exam-preparation-practice-test)
  - [HashiCorp Certified: Terraform Associate - Hands-On Labs](#hashicorp-certified-terraform-associate---hands-on-labs)
  - [Understanding the Terraform Basics](#understanding-the-terraform-basics)
  - [Use Terraform Outside of Core Workflow](#use-terraform-outside-of-core-workflow)
  - [Interact with Terraform Modules](#interact-with-terraform-modules)
  - [Use the Core Terraform Workflow.](#use-the-core-terraform-workflow)
  - [Implement and Maintain State](#implement-and-maintain-state)
  - [Read, Generate, and Modify Configuration](#read-generate-and-modify-configuration)

<br>

<hr style="height:4px;background:black">

<br>

# Terraform 

## HashiCorp Certified: Terraform Associate 2024
1. Introduction: [text](hashicorp/introduction-to-terraform.md).
2. Deploying Infrastructure with Terraform: [text](deploy-infrastructure.md)
3. Read, Generate, Modify Configurations: [text](read-generate-modify.md)
4. [Terraform Provisioners](hashicorp/terraform-provisioners.md).
5. Terraform [Modules & Workspaces](hashicorp/modules-workspaces.md). 
6. [Remote State Management](hashicorp/remote-state-management.md).
7. [Security Primer](hashicorp/security-primer.md).
8. Terraform [Cloud & Enterprise](hashicorp/cloud-enterprise.md) Capabilities. 
9. [Terraform Challenges](hashicorp/terraform-challenges.md). 

<br>

### HashiCorp Exam Preparation Practice Test
* Exam [1](exam_practise/exam1.md).
* Exam [2](exam_practise/exam2.md).
* Exam [3](exam_practise/exam3.md).

<br>

<hr style="height:4px;background:black">

<br>

## HashiCorp Certified: Terraform Associate - Hands-On Labs
Documentation:
* GitHub Repo for Supporting Files: https://github.com/btkrausen/hashicorp 
* GitHub Repo for Labs: https://github.com/btkrausen/hashicorp/tree/master/terraform/Hands-On%20Labs

<br>

<hr style="height:4px;background:black">

<br>

## Understanding the Terraform Basics
1. Terraform [Basics](basics-docs/Terraform+Basics.pdf). ([text](basics-docs/Terraform+Basics.pdf))
2. HashiCorp Configuration Language ([HCL](basics-docs/HashiCorp+Configuration+Language.pdf)).
3. Terraform [Plub-in Based Architecture](basics-docs/Terraform+Plugin+Based+Architecture.pdf). 
4. Terraform [Providor](basics-docs/Intro+to+the+Terraform+Provider+Block.pdf) Block.
5. Terraform [Resource](basics-docs/Intro+to+the+Terraform+Resource+Block.pdf) Block. 
6. Terraform [Input Variables](basics-docs/Intro+to+the+Input+Variables+Block.pdf) Block.
7. Terraform [Local Variable](basics-docs/Intro+to+the+Local+Variables+Block.pdf) Block.
8. Terraform [Data](basics-docs/Intro+to+the+Data+Block.pdf) Block.
9. Terraform [Configuration](basics-docs/Intro+to+the+Terraform+Configuration+Block.pdf) Block. 
10. Terraform [Module](basics-docs/Intro+to+the+Module+Block.pdf) Block.
11. Terraform [Output](basics-docs/Intro+to+the+Terraform+Output+Block.pdf) Block.
12. [Commenting](basics-docs/Commenting+Terraform+Code.pdf) Terraform Code.
13. Terraform Provider [Installation and Versioning](basics-docs/Terraform+Providers+Installation.pdf). 
14. Using [Multiple Terraform Providers](basics-docs/Multiple+Terraform+Providers.pdf). 
15. Generating an [SSH Key](basics-docs/Terraform+TLS+Provider.pdf) using the Terraform TLS Provider.
16. [Fetch, Version, and Upgrade](basics-docs/Fetch+Version+and+Upgrade+Terraform+Providers.pdf) Terraform Providers. 
17. Terraform [Provisioners](basics-docs/Terraform+Provisioners.pdf).

<br>

<hr style="height:4px;background:black">

<br>

## Use Terraform Outside of Core Workflow
1. [Auto Formatting](outside-core-workflow-docs/Auto+Formatting+Terraform+Code.pdf) Terraform Code.
2. Replace Resources using [Terraform Taint](outside-core-workflow-docs/Terraform+Taint+and+Replace.pdf).
3. Terraform [Import](outside-core-workflow-docs/Terraform+Import.pdf).
4. Terraform Workspaces - [OSS](outside-core-workflow-docs/Terraform+Workspaces+-+OSS.pdf).
5. Terraform [State CLI](outside-core-workflow-docs/Terraform+State.pdf).
6. [Debugging](outside-core-workflow-docs/Debugging+Terraform.pdf) Terraform. 

<br>

<hr style="height:4px;background:black">

<br>

## Interact with Terraform Modules
1. Terraform [Modules](modules-docs/Terraform+Modules.pdf).
   * [Sources](modules-docs/Terraform+Modules+Sources.pdf).
   * [Inputs and Outputs](modules-docs/Terraform+Module+Inputs+and+Outputs.pdf). 
   * [Scope](modules-docs/Terraform+Module+Scope.pdf).
   * [Public Registry](modules-docs/Terraform+Module+Registry.pdf).
   * [Versioning](modules-docs/Terraform+Module+Versions.pdf).

<br>

<hr style="height:4px;background:black">

<br>

## Use the Core Terraform Workflow.
1. Understanding the Terraform [Workflow](core-docs/Terraform+Workflow.pdf).
2. Initialising Terraform with the '[terraform init](core-docs/Terraform+Init.pdf)' command.
3. Validating Terraform Configuration with '[terraform validate](core-docs/Validating+Terraform+Configuration.pdf)'.
4. Generate and Review an Execution Plan with '[terraform plan](core-docs/Terraform+Plan.pdf)'.
5. Execute Changes to Infrastructure with '[terraform apply](core-docs/Terraform+Apply.pdf)'.
6. Delete Resources Using the '[terraform destroy](core-docs/Terraform+Destroy.pdf)' command. 

<br>

<hr style="height:4px;background:black">

<br>

## Implement and Maintain State
1. Terraform State - [Default Local Backend](documentation/implement-and-maintain-state/Terraform+State+Default+Local+Backend.pdf).
2. Terraform State [Locking](documentation/implement-and-maintain-state/Terraform+State+Locking.pdf). 
3. Terraform State - [Backend Authentication](documentation/implement-and-maintain-state/Terraform+State+Backend+Authentication.pdf).
4. Terraform State - [Backend Storage](documentation/implement-and-maintain-state/Terraform+State+Backend+Storage.pdf).
5. Terraform Remote State - [Enhanced Backend](documentation/implement-and-maintain-state/Terraform+Remote+State+Enhanced+Backend.pdf).
6. Terraform State [Migration](documentation/implement-and-maintain-state/Terraform+State+Migration.pdf).
7. Terraform State [Refresh](documentation/implement-and-maintain-state/Terraform+State+Refresh.pdf).
8. Terraform Backend [Configuration](documentation/implement-and-maintain-state/Terraform+Backend+Configuration.pdf).
9. [Sensitive Data](documentation/implement-and-maintain-state/Sensitive+Data+in+Terraform+State.pdf) in Terraform State. 

<br>

<hr style="height:4px;background:black">

<br>

## Read, Generate, and Modify Configuration
1. 