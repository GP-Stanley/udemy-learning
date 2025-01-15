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
*  Demonstration: [Installing Redis](docker-basics.md#demonstration-installing-redis).
*  [What is Docker?](docker-basics.md#what-is-docker)
*  [Using the Docker Client](docker-basics.md#using-the-docker-client).
*  [What is a Container?](docker-basics.md#what-is-a-container)

<br>

<hr style="height:4px;background:black">

<br>

# Section 2: [Manipulating Containers with the Docker Client](docker-basics.md#section-2-manipulating-containers-with-the-docker-client)
* '[Docker Run](docker-basics.md#docker-run-in-detail)' in Detail.
* [Overriding Default Commands](docker-basics.md#overriding-default-commands).
* [Listing Running Containers](docker-basics.md#listing-running-containers).
* [Container Lifecycle](docker-basics.md#container-lifecycle).
* [Restarting Stopped Containers](docker-basics.md#restarting-stopped-containers).
* [Removing Stopped Containers](docker-basics.md#removing-stopped-containers).
* [Retrieving Log Outputs](docker-basics.md#retrieving-log-outputs).
* [Stopping Containers](docker-basics.md#stopping-containers).
* [Multi-Command Containers](docker-basics.md#multi-command-containers).
* [Executing Commands in Running Containers](docker-basics.md#executing-commands-in-running-containers).
* The Purpose of the [-it Flag](docker-basics.md#the-purpose-of-the--it-flag).
* Getting a [Command Prompt in a Container](docker-basics.md#getting-a-command-prompt-in-a-container).
* Starting with a [Shell](docker-basics.md#starting-with-a-shell).
* [Container Isolation](docker-basics.md#container-isolation).

<br>

<hr style="height:4px;background:black">

<br>

# Section 3: [Building Custom Images Through Docker Server](docker-basics.md#section-3-building-custom-images-through-docker-server)
* [Creating Docker Images](docker-basics.md#creating-docker-images).
* [Buildkit](docker-basics.md#buildkit-for-docker-desktop) for Docker Desktop.
* [Dockerfile Teardown](docker-basics.md#dockerfile-teardown).
* [What's a Base Image?](docker-basics.md#whats-a-base-image)
* The [Build Process](docker-basics.md#the-build-process-in-detail) in Detail.
* [A Brief Recap](docker-basics.md#a-brief-recap).
* [Rebuilds with Cache](docker-basics.md#rebuilds-with-cache).
* [Tagging an Image](docker-basics.md#tagging-an-image).
* [Manual Image Generation](docker-basics.md#manual-image-generation-with-docker-commit) with Docker Commit.

<br>

<hr style="height:4px;background:black">

<br>

# Section 5: [Docker Compose with Multiple Local Containers](docker-compose.md#section-5-docker-compose-with-multiple-local-containers)
* [App Overview](docker-compose.md#app-overview).
* [Assembling a Dockerfile](docker-compose.md#assembling-a-dockerfile).
* Introducing [Docker Compose](docker-compose.md#introducing-docker-compose).
* Docker Compose [Files](docker-compose.md#docker-compose-files).
* [Networking](docker-compose.md#networking-with-docker-compose) with Docker Compose.
* [Stopping Docker Compose Containers](docker-compose.md#stopping-docker-compose-containers).
* [Container Maintenance](docker-compose.md#container-maintenance-with-compose) with Compose.
* [Automatic Container Restarts](docker-compose.md#automatic-container-restarts).
* [Container Status](docker-compose.md#container-status-with-docker-compose) with Docker Compose.

<br>

<hr style="height:4px;background:black">

<br>

# Section 6: [Creating a Production-Grade Workflow](prod-grade-workflow.md#section-6-creating-a-production-grade-workflow)
* [Development Workflow](prod-grade-workflow.md#development-workflow).
* [Flow Specifics](prod-grade-workflow.md#flow-specifics).
* [Docker's Purpose](prod-grade-workflow.md#dockers-purpose).
* [Project Generation](prod-grade-workflow.md#project-generation).
* [Necessary Commands](prod-grade-workflow.md#necessary-commands).
* [Creating the Dev Dockerfile](prod-grade-workflow.md#creating-the-dev-dockerfile).
* [Duplicating Dependencies](prod-grade-workflow.md#duplicating-dependencies).
* [Starting the Container](prod-grade-workflow.md#starting-the-container).
* [Docker Volumes](prod-grade-workflow.md#docker-volumes).
* [Bookmarking Volumes](prod-grade-workflow.md#bookmarking-volumes).
* [Shorthand](prod-grade-workflow.md#shorthand-with-docker-compose) with Docker Compose.
* [Overriding Dockerfile Selection](prod-grade-workflow.md#overriding-dockerfile-selection).
* [Do We Need Copy?](prod-grade-workflow.md#do-we-need-copy)
* [Executing Tests](prod-grade-workflow.md#executing-tests).
* [Live Updating Tools](prod-grade-workflow.md#live-updating-tools).
* [Docker Compose for Running Tests](prod-grade-workflow.md#docker-compose-for-running-tests).
* [Shortcomings on Testing](prod-grade-workflow.md#shortcomings-on-testing).
* [Need for Nginx](prod-grade-workflow.md#nginx-preparing-docker-container-for-production).
* [Multi-Step Docker Builds](prod-grade-workflow.md#multi-step-docker-builds-using-nginx-for-production-environment).
* [Implementing Multi-Step Builds](prod-grade-workflow.md#implementing-multi-step-builds-for-production-dockerfile).
* [Running Nginx](prod-grade-workflow.md#running-nginx).

<br>

<hr style="height:4px;background:black">

<br>

# Section 7: [Continuous Integration and Deployment with AWS](ci-and-deployment.md#section-7-continuous-integration-and-deployment-with-aws)
* [Services Overview](ci-and-deployment.md#services-overview).
* [GitHub Setup](ci-and-deployment.md#github-setup).
* [Travis CI Setup](ci-and-deployment.md#travis-ci-setup).
* [Travis YAML File Configuration](ci-and-deployment.md#travis-yaml-file-configuration).
* More Travis CI [Setup](ci-and-deployment.md#more-travis-ci-setup).
* [Automatic Build Creation](ci-and-deployment.md#automatic-build-creation-committing-changes-and-pushing-to-github).
* [AWS Elastic Beanstalk](ci-and-deployment.md#aws-elastic-beanstalk-setting-up-automatic-deployment-to-aws).
* Elastic Beanstalk [Setup and Configuration](ci-and-deployment.md#elastic-beanstalk-setup-and-configuration).
* More on [Elastic Beanstalk](ci-and-deployment.md#more-on-elastic-beanstalk).
* Travis [Config for Deployment](ci-and-deployment.md#travis-config-for-deployment).
* [Automated Deployments](ci-and-deployment.md#automated-deployments).
* [Exposing Ports](ci-and-deployment.md#exposing-ports-through-the-dockerfile) Through the Dockerfile.
* [Workflow With GitHub](ci-and-deployment.md#workflow-with-github).
* [Merging Pull Requests and Deploying with Travis CI](ci-and-deployment.md#merging-pull-requests-and-deploying-with-travis-ci).
* [Reviewing the Deployment Workflow](ci-and-deployment.md#reviewing-the-deployment-workflow).
* [Environment Clean-Up](ci-and-deployment.md#environment-clean-up).
* [AWS Configuration Cheat Sheet](ci-and-deployment.md#aws-configuration-cheat-sheet).

<br>

<hr style="height:4px;background:black">

<br>

# Section 8: [Building a Multi-Container Application](multi-container-app.md#section-8-building-a-multi-container-application)
* [Single Container Deployment Issues](multi-container-app.md#single-container-deployment-issues).
* Application Overview: [Building a Multi-Container Application](multi-container-app.md#building-a-multi-container-application-fibonacci-calculator).
* [Application Architecture](multi-container-app.md#application-architecture).
* [Worker Process Setup](multi-container-app.md#worker-process-setup).
* [Express API Setup](multi-container-app.md#express-api-setup).
* [Connecting to Postgress](multi-container-app.md#connecting-to-postgress).
* More [Express API Setup](multi-container-app.md#more-express-api-setup).
* [Fetching data](multi-container-app.md#fetching-data-in-the-react-app) in the React App.
* [Rendering Logic](multi-container-app.md#rendering-logic-in-the-app) in the App.
* [Routing](multi-container-app.md#routing-in-the-react-app) in the React App.

<br>

<hr style="height:4px;background:black">

<br>

# Section 9: ["Dockerizing" Multiple Services](multiple-services.md#section-9-dockerizing-multiple-services)
* [Dockerizing a React App](multiple-services.md#dockerizing-a-react-app---again) - Again!
* [Dockerizing Generic Node Apps](multiple-services.md#dockerizing-generic-node-apps).
* [Adding Postgres as a Service](multiple-services.md#adding-postgres-as-a-service).
* [Docker-compose Configuration](multiple-services.md#docker-compose-configuration).
* [Environment Variables with Docker Compose](multiple-services.md#environment-variables-with-docker-compose).
* [Required Worker Environment Variables](multiple-services.md#required-worker-environment-variables).
* [The Worker and Client Services](multiple-services.md#the-worker-and-client-services).
* [Nginx Path Routing](multiple-services.md#nginx-path-routing).
* [Routing with Nginx](multiple-services.md#routing-with-nginx).
* [Building a Custom Nginx Image](multiple-services.md#building-a-custom-nginx-image).
* [Starting Up Docker Compose](multiple-services.md#starting-up-docker-compose).
* [Nginx connect() failed](multiple-services.md#nginx-connect-failed---connection-refused-while-connecting-to-upstream) - Connection refused while connecting to upstream.
* [Troubleshooting Startup Bugs](multiple-services.md#troubleshooting-startup-bugs).
* [Openinig Websocket Connections](multiple-services.md#openinig-websocket-connections).

<br>

<hr style="height:4px;background:black">

<br>

# Section 10: [A Continuous Integration Workflow for Multiple Images](continuous-integration-multi-images.md#section-10-a-continuous-integration-workflow-for-multiple-images)
* [Production Multi-Container Deployments](continuous-integration-multi-images.md#production-multi-container-deployments).
* [Production Dockerfiles](continuous-integration-multi-images.md#production-dockerfiles).
* [Multiple Nginx Instances](continuous-integration-multi-images.md#multiple-nginx-instances).
* [Nginx Fix](continuous-integration-multi-images.md#nginx-fix-fo-react-router) fo React Router.
* [Altering Nginx's Listen Port](continuous-integration-multi-images.md#altering-nginxs-listen-port).
* [Travis Configuration Setup](continuous-integration-multi-images.md#travis-configuration-setup).
* [GitHub and Travis CI Setup](continuous-integration-multi-images.md#github-and-travis-ci-setup).
* [Pushing Images to Docker Hub](continuous-integration-multi-images.md#pushing-images-to-docker-hub).

<br>

<hr style="height:4px;background:black">

<br>

# Section 11: [Multi-Container Deployments to AWS](aws-multi-container-deployments.md#section-11-multi-container-deployments-to-aws)
* [Multi-Container Definition Files](aws-multi-container-deployments.md#multi-container-definition-files).
* [Finding Docs on Container Definitions](aws-multi-container-deployments.md#finding-docs-on-container-definitions). 
* [Adding Container Definitions to DockerRun](aws-multi-container-deployments.md#adding-container-definitions-to-dockerrun).
* More [Container Definitions](aws-multi-container-deployments.md#more-container-definitions).
* [Forming Container Links](aws-multi-container-deployments.md#forming-container-links).
* [Creating the Elastic Beanstalk Environment](aws-multi-container-deployments.md#creating-the-elastic-beanstalk-environment).
* [AWS Configuration Sheet](aws-multi-container-deployments.md#aws-configuration).
  * Elastic Beanstalk [Application Creation](aws-multi-container-deployments.md#elastic-beanstalk-application-creation).
  * [RDS Database Creation](aws-multi-container-deployments.md#rds-database-creation).
  * [ElastiCache Redis Creation](aws-multi-container-deployments.md#elasticache-redis-creation).
  * Creating a [Custom Security Group](aws-multi-container-deployments.md#creating-a-custom-security-group).
  * [Applying Security Groups to ElastiCache](aws-multi-container-deployments.md#applying-security-groups-to-elasticache).
  * [Applying Security Groups to RDS](aws-multi-container-deployments.md#applying-security-groups-to-rds).
  * [Applying Security Groups to Elastic Beanstalk](aws-multi-container-deployments.md#applying-security-groups-to-elastic-beanstalk).
  * [Add AWS configuration details to .travis.yml file's deploy script](aws-multi-container-deployments.md#add-aws-configuration-details-to-travisyml-files-deploy-script).
  * [Setting Environment Variables](aws-multi-container-deployments.md#setting-environment-variables).
  * [IAM Keys for Deployment](aws-multi-container-deployments.md#iam-keys-for-deployment).
  * [AWS Keys in Travis](aws-multi-container-deployments.md#aws-keys-in-travis).
  * [Deploying App](aws-multi-container-deployments.md#deploying-app).
* [Managed Data Service Providers](aws-multi-container-deployments.md#managed-data-service-providers). 
* Overview of [AWS VPC's and Security Groups](aws-multi-container-deployments.md#overview-of-aws-vpcs-and-security-groups).
* [RDS Database Creation](aws-multi-container-deployments.md#rds-database-creation-1).
* [ElastiCache Redis Creation](aws-multi-container-deployments.md#elasticache-redis-creation-1).
* [Creating a Custom Security Group](aws-multi-container-deployments.md#creating-a-custom-security-group-1).
* [Applying Security Groups to Resources](aws-multi-container-deployments.md#applying-security-groups-to-resources).
* [Setting Environment Variables](aws-multi-container-deployments.md#setting-environment-variables-1).
* [IAM Keys for Deployment](aws-multi-container-deployments.md#iam-keys-for-deployment-1).
* [Travis Deploy Script](aws-multi-container-deployments.md#travis-deploy-script).
* [Container Memory Allocations](aws-multi-container-deployments.md#container-memory-allocations).
* [Verifying Deployment](aws-multi-container-deployments.md#verifying-deployment).

<br>

<hr style="height:4px;background:black">

<br>
