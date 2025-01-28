- [Section 12: Onwards to Kubernetes!](#section-12-onwards-to-kubernetes)
- [Section 13: Maintaining Sets of Containers with Deployments](#section-13-maintaining-sets-of-containers-with-deployments)
- [Section 14: A Multi-Container App with Kubernetes](#section-14-a-multi-container-app-with-kubernetes)
- [Section 15: Handling Traffic with Ingress Controllers](#section-15-handling-traffic-with-ingress-controllers)
- [Section 16: Kubernetes Production Deployment](#section-16-kubernetes-production-deployment)
- [Section 17: HTTPS Setup with Kubernetes](#section-17-https-setup-with-kubernetes)
- [Section 18: Local Development with Skaffold](#section-18-local-development-with-skaffold)

<br>

<hr style="height:4px;background:black">

<br>

# Section 12: [Onwards to Kubernetes!](guide-to-kubernetes.md#section-12-onwards-to-kubernetes)
* [The Why's and What's of Kubernetes](guide-to-kubernetes.md#the-whys-and-whats-of-kubernetes).
* [Kubernetes in Development and Production](guide-to-kubernetes.md#kubernetes-in-development-and-production).
* Kubernetes Setup and Installation.
  * Docker Desktop's Kubernetes [Setup and Installation - macOS](guide-to-kubernetes.md#docker-desktops-kubernetes-setup-and-installation---macos).
  * [Minikube Install Setup Info - macOS](guide-to-kubernetes.md#minikube-install-and-setup-info---macos).
  * Docker Desktop's Kubernetes [Setup and Installation - Windows](guide-to-kubernetes.md).
  * [Minikube Setup on Windows](guide-to-kubernetes.md#minikube-setup-on-windows). 
  * [Minikube Setup on Linux](guide-to-kubernetes.md#minikube-setup-on-linux).
* [Mapping Existing Knowledge](guide-to-kubernetes.md#mapping-existing-knowledge).
  * Quick Note to [Prevent an Error](guide-to-kubernetes.md#quick-note-to-prevent-an-error).
* [Adding Configuration Files](guide-to-kubernetes.md#adding-configuration-files).
* [Object Types and API Versions](guide-to-kubernetes.md#object-types-and-api-versions).
* [Running Containers in Pods](guide-to-kubernetes.md#running-containers-in-pods). 
* [Service Config Files in Depth](guide-to-kubernetes.md#service-congif-files-in-depth).
* [Connecting to Running Containers](guide-to-kubernetes.md#connecting-to-running-containers).
* The Entire [Deployment Flow](guide-to-kubernetes.md#the-entire-deployment-flow).
* [Imperative vs Declarative Deployments](guide-to-kubernetes.md#imperative-vs-declarative-deployments).

<br>

<hr style="height:4px;background:black">

<br>

# Section 13: [Maintaining Sets of Containers with Deployments](maintaining-sets-containers.md#section-13-maintaining-sets-of-containers-with-deployments)
* [Updating Existing Objects](maintaining-sets-containers.md#updating-existing-objects).
* [Declarative Updates in Action](maintaining-sets-containers.md#declarative-updates-in-action).
* [Limitations in Config Updates](maintaining-sets-containers.md#limitations-in-config-updates).
* [Running Containers with Delpoyments](maintaining-sets-containers.md#running-containers-with-delpoyments).
* [Deployment Configuration Files](maintaining-sets-containers.md#deployment-configuration-files).
* Walking Through the [Deployment Config](maintaining-sets-containers.md#walking-through-the-deployment-config).
* [Applying a Deployment](maintaining-sets-containers.md#applying-a-deployment).
* [Why Use Services?](maintaining-sets-containers.md#why-use-services)
* [Scaling and Changing Deployments](maintaining-sets-containers.md#scaling-and-changing-deployments).
* [Updating Deployment Images](maintaining-sets-containers.md#updating-deployment-images).
* [Rebuilding the Client Image](maintaining-sets-containers.md#rebuilding-the-client-image). 
* [Triggering Deployment Updates](maintaining-sets-containers.md#triggering-deployment-updates).
* [Imperatively Updating a Deployment's Image](maintaining-sets-containers.md#imperatively-updating-a-deployments-image).
* [Multiple Docker Installations](maintaining-sets-containers.md#multiple-docker-installations).
* [Reconfiguring Docker CLI](maintaining-sets-containers.md#reconfiguring-docker-cli).
* [Why Mess with Docker in the Node?](maintaining-sets-containers.md#why-mess-with-docker-in-the-node)

<br>

<hr style="height:4px;background:black">

<br>

# Section 14: [A Multi-Container App with Kubernetes](multi-container-app.md#section-14-a-multi-container-app-with-kubernetes)
* [The Path to Production](multi-container-app.md#the-path-to-production).
* [Recreating the Deployment](multi-container-app.md#recreating-the-deployment).
* [NodePort vs ClusterIP Services](multi-container-app.md#nodeport-vs-clusterip-services).
* [The ClusterIP Config](multi-container-app.md#the-clusterip-config).
* [Applying Multiple Files with Kubectl](multi-container-app.md#applying-multiple-files-with-kubectl).
* [Expess API Deployment Config](multi-container-app.md#expess-api-deployment-config).
* [Cluster IP for the Express API](multi-container-app.md#cluster-ip-for-the-express-api).
* [Combining Config into Single Files](multi-container-app.md#combining-config-into-single-files).
* [The Worker Deployment](multi-container-app.md#the-worker-deployment).
* [Reapplying a Batch of Config Files](multi-container-app.md#reapplying-a-batch-of-config-files).
* [Creating and Applying Redis Config](multi-container-app.md#creating-and-applying-redis-config).
* [Last Set of Borning Config!](multi-container-app.md#last-set-of-borning-config)
* [The Need for Volumes with Databases](multi-container-app.md#the-need-for-volumes-with-databases).
* [Kubernetes Volumes](multi-container-app.md#kubernetes-volumes).
* [Volumes vs Persistent Volumes](multi-container-app.md#volumes-vs-persistent-volumes).
* [Persistent Volumes vs Persistent Volume Claims](multi-container-app.md#persistent-volumes-vs-persistent-volume-claims).
* [Claim Config Files](multi-container-app.md#claim-config-files).
* [Persistent Volume Access Modes](multi-container-app.md#persistent-volume-access-modes).
* [Where Does Kubernetes Allocate Persistent Volumes?](multi-container-app.md#where-does-kubernetes-allocate-persistent-volumes)
* [Designating a PVC in a Pod Template](multi-container-app.md#designating-a-pvc-in-a-pod-template).
* [Applying a PVC](multi-container-app.md#applying-a-pvc).
* [Definging Environment Variables](multi-container-app.md#definging-environment-variables).
* [Adding Environment Variables to Config](multi-container-app.md#adding-environment-variables-to-config).
* [Creating an Encoded Secret](multi-container-app.md#creating-an-encoded-secret).
* [Passing Secrets as Environment Variables](multi-container-app.md#passing-secrets-as-environment-variables).

<br>

<hr style="height:4px;background:black">

<br>

# Section 15: [Handling Traffic with Ingress Controllers](ingress-controllers.md#section-15-handling-traffic-with-ingress-controllers)
* [Load Balancer Services](ingress-controllers.md#load-balancer-services).
* A Quick Note on [Ingresses](ingress-controllers.md#a-quick-note-on-ingresses).
* One Other [Quick Note!](ingress-controllers.md#one-other-quick-note)
* [Behind the Scenes of Ingress](ingress-controllers.md#behind-the-scenes-of-ingress).
* [More Behind the Scenes of Ingress](ingress-controllers.md#more-behind-the-scenes-of-ingress).
* [Setting Up Ingress Locally with Minikube](ingress-controllers.md#setting-up-ingress-locally-with-minikube).
* [Creating the Ingress Configuration](ingress-controllers.md#creating-the-ingress-configuration).
* [Testing Ingress Locally](ingress-controllers.md#testing-ingress-locally).
* The [Minikube Dashboard](ingress-controllers.md#the-minikube-dashboard).

<br>

<hr style="height:4px;background:black">

<br>

# Section 16: [Kubernetes Production Deployment](production-deployment.md#section-16-kubernetes-production-deployment)
* The [Deployment Process](production-deployment.md#the-deployment-process).
* [Google Cloud vs AWS for Kubernetes](production-deployment.md#google-cloud-vs-aws-for-kubernetes).
* [Creating a Git Repo](production-deployment.md#creating-a-git-repo).
* [Linking the GitHub Repo to Travis](production-deployment.md#linking-the-github-repo-to-travis).
* [Creating a Google Cloud Project](production-deployment.md#creating-a-google-cloud-project).
* [Linking a Billing Account](production-deployment.md#linking-a-billing-account).
* [Kubernetes Engine Init](production-deployment.md#kubernetes-engine-init).
* [Creating a Cluster with Google Cloud](production-deployment.md#creating-a-cluster-with-google-cloud).
* [Kubernetes Dashboard on Google Cloud](production-deployment.md#kubernetes-dashboard-on-google-cloud).
* [Travis Deployment Overview](production-deployment.md#travis-deployment-overview).
* [Installing the Google Cloud SDK](production-deployment.md#installing-the-google-cloud-sdk).
* [Generating a Service Account](production-deployment.md#generating-a-service-account). 
* [Running Travis CLI in a Container](production-deployment.md#running-travis-cli-in-a-container).
* [Encrypting a Service Account File](production-deployment.md#encrypting-a-service-account-file).
* More [Google Cloud CLI Config](production-deployment.md#more-google-cloud-cli-config).
* [Running Tests with Travis](production-deployment.md#running-tests-with-travis).
* [Custom Deployment Providers](production-deployment.md#custom-deployment-providers).
* [Unique Deployment Images](production-deployment.md#unique-deployment-images).
* [Unique Tags for Built Images](production-deployment.md#unique-tags-for-built-images).
* [Updating the Deployment Script](production-deployment.md#updating-the-deployment-script).
* [Configuring the GCloud CLI on Cloud Console](production-deployment.md#configuring-the-gcloud-cli-on-cloud-console).
* [Creating a Secret on Google Cloud](production-deployment.md#creating-a-secret-on-google-cloud).
* [Helm Setup](production-deployment.md#helm-setup).
* [Ingress-Nginx with Helm](production-deployment.md#ingress-nginx-with-helm).
* [The Result of Ingress-Nginx](production-deployment.md#the-result-of-ingress-nginx).
* [Deployment](production-deployment.md#deployment).
* [Verifying Deployment](production-deployment.md#verifying-deployment).
* [A Workflow for Changing in Prod](production-deployment.md#a-workflow-for-changing-in-prod).
* [Merging a PR for Deployment](production-deployment.md#merging-a-pr-for-deployment).

<br>

<hr style="height:4px;background:black">

<br>

# Section 17: [HTTPS Setup with Kubernetes](https-setup.md#section-17-https-setup-with-kubernetes)
* [HTTPS Setup Overview](https-setup.md#https-setup-overview).
* [Domain Purchase](https-setup.md#domain-purchase).
* [Domain Name Setup](https-setup.md#domain-name-setup).
* [Cert Manager Install](https-setup.md#cert-manager-install).
* [How to Wire Up Cert Manager](https-setup.md#how-to-wire-up-cert-manager).
* [Issuer Config File](https-setup.md#issuer-config-file).
* [Certificate Config File](https-setup.md#certificate-config-file).
* [Deploying Changes](https-setup.md#deploying-changes).
* [Verifying the Certificate](https-setup.md#verifying-the-certificate).
* [Ingress Config for HTTPS](https-setup.md#ingress-config-for-https).
* [It Worked!](https-setup.md#it-worked)
* [Google Cloud Clean Up](https-setup.md#google-cloud-clean-up).
* [Local Environment Clean Up](https-setup.md).

<br>

<hr style="height:4px;background:black">

<br>

# Section 18: [Local Development with Skaffold](local-dev-skaffold.md#section-18-local-development-with-skaffold)
* Awkward [Local Development](local-dev-skaffold.md#awkward-local-development).
* [Installing Skaffold](local-dev-skaffold.md#installing-skaffold).
* [The Skaffold Config File](local-dev-skaffold.md#the-skaffold-config-file).
* [Live Sync Changes](local-dev-skaffold.md#live-sync-changes).
* [Automatic Shutdown](local-dev-skaffold.md#automatic-shutdown-managing-deployments-with-skaffold).
* [Testing Live Sync with the API Server](local-dev-skaffold.md#testing-live-sync-with-the-api-server).

<br>

<hr style="height:4px;background:black">

<br>