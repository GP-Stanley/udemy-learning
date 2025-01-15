- [Section 1: Dive into Docker](#section-1-dive-into-docker)
- [Section 2: Manipulating Containers with the Docker Client](#section-2-manipulating-containers-with-the-docker-client)
- [Section 3: Building Custom Images Through Docker Server](#section-3-building-custom-images-through-docker-server)
- [Section 5: Docker Compose with Multiple Local Containers](#section-5-docker-compose-with-multiple-local-containers)
- [Section 6: Creating a Production-Grade Workflow](#section-6-creating-a-production-grade-workflow)
- [Section 7: Continuous Integration and Deployment with AWS](#section-7-continuous-integration-and-deployment-with-aws)
- [Section 8: Building a Multi-Container Application](#section-8-building-a-multi-container-application)
- [Section 9: "Dockerizing" Multiple Services](#section-9-dockerizing-multiple-services)
- [Section 10: A Continuous Integration Workflow for Multiple Images](#section-10-a-continuous-integration-workflow-for-multiple-images)
- [Section 11: Multi-Container Deployments to AWS](#section-11-multi-container-deployments-to-aws)


<br>

<hr style="height:4px;background:black">

<br>

GitHub reference: https://github.com/StephenGrider/DockerCasts

<br>

# Section 1: [Dive into Docker](docker-basics.md#section-1-dive-into-docker)
*  [Why Use Docker?](docker-basics.md#why-use-docker)
*  Demonstration: [Installing Redis](docker-basics.md#demonstration-installing-redis)
*  [What is Docker?](docker-basics.md#what-is-docker)
*  [Using the Docker Client](docker-basics.md#using-the-docker-client)
*  [What is a Container?](docker-basics.md#what-is-a-container)

<br>

<hr style="height:4px;background:black">

<br>

# Section 2: [Manipulating Containers with the Docker Client](docker-basics.md#section-2-manipulating-containers-with-the-docker-client)
* 'Docker Run' in Detail
* Overriding Default Commands
* Listing Running Containers
* Container Lifecycle
* Restarting Stopped Containers
* Removing Stopped Containers
* Retrieving Log Outputs
* Stopping Containers
* Multi-Command Containers
* Executing Commands in Running Containers
* The Purpose of the -it Flag
* Getting a Command Prompt in a Container
* Starting with a Shell
* Container Isolation

<br>

<hr style="height:4px;background:black">

<br>

# Section 3: [Building Custom Images Through Docker Server](docker-basics.md#section-3-building-custom-images-through-docker-server)
* Creating Docker Images
* Buildkit for Docker Desktop
* Dockerfile Teardown
* What's a Base Image?
* The Build Process in Detail
* A Brief Recap
* Rebuilds with Cache
* Tagging an Image
* Manual Image Generation with Docker Commit

<br>

<hr style="height:4px;background:black">

<br>

# Section 5: [Docker Compose with Multiple Local Containers](docker-compose.md#section-5-docker-compose-with-multiple-local-containers)
* App Overview.
* Assembling a Dockerfile.
* Introducing Docker Compose.
* Docker Compose Files.
* Networking with Docker Compose.
* Stopping Docker Compose Containers.
* Container Maintenance with Compose.
* Automatic Container Restarts.
* Container Status with Docker Compose.

<br>

<hr style="height:4px;background:black">

<br>

# Section 6: [Creating a Production-Grade Workflow](prod-grade-workflow.md#section-6-creating-a-production-grade-workflow)
* Development Workflow.
* Flow Specifics.
* Docker's Purpose.
* Project Generation.
* Necessary Commands.
* Creating the Dev Dockerfile.
* Duplicating Dependencies.
* Starting the Container.
* Docker Volumes.
* Bookmarking Volumes.
* Shorthand with Docker Compose.
* Overriding Dockerfile Selection.
* Do We Need Copy?
* Executing Tests.
* Live Updating Tools.
* Docker Compose for Running Tests.
* Shortcomings on Testing.
* Need for Nginx.
* Multi-Step Docker Builds.
* Implementing Multi-Step Builds.
* Running Nginx.

<br>

<hr style="height:4px;background:black">

<br>

# Section 7: [Continuous Integration and Deployment with AWS](ci-and-deployment.md#section-7-continuous-integration-and-deployment-with-aws)
* Services Overview.
* GitHub Setup.
* Travis CI Setup.
* Travis YAML File Configuration.
* More Travis CI Setup.
* Automatic Build Creation.
* AWS Elastic Beanstalk.
* Elastic Beanstalk Setup and Configuration.
* More on Elastic Beanstalk.
* Travis Config for Deployment.
* Automated Deployments.
* Exposing Ports Through the Dockerfile.
* Workflow With GitHub.
* Merging Pull Requests and Deploying with Travis CI.
* Reviewing the Deployment Workflow.
* Environment Clean-Up.
* AWS Configuration Cheat Sheet.

<br>

<hr style="height:4px;background:black">

<br>

# Section 8: [Building a Multi-Container Application](multi-container-app.md#section-8-building-a-multi-container-application)
* Single Container Deployment Issues.
* Application Overview: Building a Multi-Container Application.
* Application Architecture.
* Worker Process Setup.
* Express API Setup.
* Connecting to Postgress.
* More Express API Setup.
* Fetching data in the React App.
* Rendering Logic in the App.
* Routing in the React App.

<br>

<hr style="height:4px;background:black">

<br>

# Section 9: ["Dockerizing" Multiple Services](multiple-services.md#section-9-dockerizing-multiple-services)
* Dockerizing a React App - Again!
* Dockerizing Generic Node Apps.
* Adding Postgres as a Service.
* Docker-compose Configuration.
* Environment Variables with Docker Compose.
* Required Worker Environment Variables.
* The Worker and Client Services.
* Nginx Path Routing.
* Routing with Nginx.
* Building a Custom Nginx Image.
* Starting Up Docker Compose.
* Nginx connect() failed - Connection refused while connecting to upstream.
* Troubleshooting Startup Bugs.
* Openinig Websocket Connections.

<br>

<hr style="height:4px;background:black">

<br>

# Section 10: [A Continuous Integration Workflow for Multiple Images](continuous-integration-multi-images.md#section-10-a-continuous-integration-workflow-for-multiple-images)
* Production Multi-Container Deployments.
* Production Dockerfiles.
* Multiple Nginx Instances.
* Nginx Fix fo React Router.
* Altering Nginx's Listen Port.
* Travis Configuration Setup.
* GitHub and Travis CI Setup.
* Pushing Images to Docker Hub.

<br>

<hr style="height:4px;background:black">

<br>

# Section 11: [Multi-Container Deployments to AWS](aws-multi-container-deployments.md#section-11-multi-container-deployments-to-aws)
* Multi-Container Definition Files.
* Finding Docs on Container Definitions. 
* Adding Container Definitions to DockerRun.
* More Container Definitions.
* Forming Container Links.
* Creating the Elastic Beanstalk Environment.
* AWS Configuration Sheet.
  * Elastic Beanstalk Application Creation.
  * RDS Database Creation.
  * ElastiCache Redis Creation.
  * Creating a Custom Security Group.
  * Applying Security Groups to ElastiCache.
  * Applying Security Groups to RDS.
  * Applying Security Groups to Elastic Beanstalk.
  * Add AWS configuration details to .travis.yml file's deploy script.
  * Setting Environment Variables.
  * IAM Keys for Deployment.
  * AWS Keys in Travis.
  * Deploying App.
* Managed Data Service Providers. 
* Overview of AWS VPC's and Security Groups.
* RDS Database Creation.
* ElastiCache Redis Creation.
* Creating a Custom Security Group.
* Applying Security Groups to Resources.
* Setting Environment Variables.
* IAM Keys for Deployment.
* Travis Deploy Script.
* Container Memory Allocations.
* Verifying Deployment.



