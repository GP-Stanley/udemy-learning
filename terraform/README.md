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
  - [Understand HCP Terraform (Terraform Cloud) Capabilities](#understand-hcp-terraform-terraform-cloud-capabilities)

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
1. Terraform [Basics](documentation/basics-docs/Terraform+Basics.pdf). 
2. HashiCorp Configuration Language ([HCL](documentation/basics-docs/HashiCorp+Configuration+Language.pdf)).
3. Terraform [Plub-in Based Architecture](documentation/basics-docs/Terraform+Plugin+Based+Architecture.pdf). 
4. Terraform [Providor](documentation/basics-docs/Intro+to+the+Terraform+Provider+Block.pdf) Block.
5. Terraform [Resource](documentation/basics-docs/Intro+to+the+Terraform+Resource+Block.pdf) Block. 
6. Terraform [Input Variables](documentation/basics-docs/Intro+to+the+Input+Variables+Block.pdf) Block.
7. Terraform [Local Variable](documentation/basics-docs/Intro+to+the+Local+Variables+Block.pdf) Block.
8. Terraform [Data](documentation/basics-docs/Intro+to+the+Data+Block.pdf) Block.
9. Terraform [Configuration](documentation/basics-docs/Intro+to+the+Terraform+Configuration+Block.pdf) Block. 
10. Terraform [Module](documentation/basics-docs/Intro+to+the+Module+Block.pdf) Block.
11. Terraform [Output](documentation/basics-docs/Intro+to+the+Terraform+Output+Block.pdf) Block.
12. [Commenting](documentation/basics-docs/Commenting+Terraform+Code.pdf) Terraform Code.
13. Terraform Provider [Installation and Versioning](documentation/basics-docs/Terraform+Providers+Installation.pdf). 
14. Using [Multiple Terraform Providers](documentation/basics-docs/Multiple+Terraform+Providers.pdf). 
15. Generating an [SSH Key](documentation/basics-docs/Terraform+TLS+Provider.pdf) using the Terraform TLS Provider.
16. [Fetch, Version, and Upgrade](documentation/basics-docs/Fetch+Version+and+Upgrade+Terraform+Providers.pdf) Terraform Providers. 
17. Terraform [Provisioners](documentation/basics-docs/Terraform+Provisioners.pdf).

<br>

<hr style="height:4px;background:black">

<br>

## Use Terraform Outside of Core Workflow
1. [Auto Formatting](documentation/outside-core-workflow-docs/Auto+Formatting+Terraform+Code.pdf) Terraform Code.
2. Replace Resources using [Terraform Taint](documentation/outside-core-workflow-docs/Terraform+Taint+and+Replace.pdf).
3. Terraform [Import](documentation/outside-core-workflow-docs/Terraform+Import.pdf).
4. Terraform Workspaces - [OSS](documentation/outside-core-workflow-docs/Terraform+Workspaces+-+OSS.pdf).
5. Terraform [State CLI](documentation/outside-core-workflow-docs/Terraform+State.pdf).
6. [Debugging](documentation/outside-core-workflow-docs/Debugging+Terraform.pdf) Terraform. 

<br>

<hr style="height:4px;background:black">

<br>

## Interact with Terraform Modules
1. Terraform [Modules](documentation/modules-docs/Terraform+Modules.pdf).
   * [Sources](documentation/modules-docs/Terraform+Modules+Sources.pdf).
   * [Inputs and Outputs](documentation/modules-docs/Terraform+Module+Inputs+and+Outputs.pdf). 
   * [Scope](documentation/modules-docs/Terraform+Module+Scope.pdf).
   * [Public Registry](documentation/modules-docs/Terraform+Module+Registry.pdf).
   * [Versioning](documentation/modules-docs/Terraform+Module+Versions.pdf).

<br>

<hr style="height:4px;background:black">

<br>

## Use the Core Terraform Workflow.
1. Understanding the Terraform [Workflow](documentation/core-docs/Terraform+Workflow.pdf).
2. Initialising Terraform with the '[terraform init](documentation/core-docs/Terraform+Init.pdf)' command.
3. Validating Terraform Configuration with '[terraform validate](documentation/core-docs/Validating+Terraform+Configuration.pdf)'.
4. Generate and Review an Execution Plan with '[terraform plan](documentation/core-docs/Terraform+Plan.pdf)'.
5. Execute Changes to Infrastructure with '[terraform apply](documentation/core-docs/Terraform+Apply.pdf)'.
6. Delete Resources Using the '[terraform destroy](documentation/core-docs/Terraform+Destroy.pdf)' command. 

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
1. [Local Variables](documentation/configuration/Terraform+Local+Values.pdf).
2. [Input Variables](documentation/configuration/Terraform+Variables.pdf).
3. Terraform [Outputs](documentation/configuration/Terraform+Outputs.pdf).
4. Variable [Validation and Suppression](documentation/configuration/Variable+Validation+and+Suppression.pdf).
5. [Secure Secrets](documentation/configuration/Secure+Secrets+in+Terraform+Code.pdf) in Terraform Code.
6. Variable [Collection and Structure](documentation/configuration/Terraform+Collections+and+Types.pdf) Types.
7. Working with [Data Blocks](documentation/configuration/Working+with+Data+Blocks.pdf).
8. Terraform [Built-in](documentation/configuration/Terraform+Built-in+Functions.pdf) Functions.
9. [Dynamic Blocks](documentation/configuration/Terraform+Dynamic+Blocks.pdf).
10. Terraform [Graph](documentation/configuration/Terraform+Graph.pdf).
11. Terraform [Resource Lifecycles](documentation/configuration/Terraform+Lifecycle+Rules.pdf).

<br>

<hr style="height:4px;background:black">

<br>

## Understand HCP Terraform (Terraform Cloud) Capabilities
1. 