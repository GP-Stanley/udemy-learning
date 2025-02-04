- [Application Developer](#application-developer)
  - [Core Concepts](#core-concepts)
  - [Configuration](#configuration)
  - [Multi-Container Pods](#multi-container-pods)
  - [Observability.](#observability)
  - [POD Design](#pod-design)
  - [Services \& Networking](#services--networking)
  - [State Persistence](#state-persistence)
  - [Security](#security)
  - [Helm Fundamentals](#helm-fundamentals)

<br>

<hr style="height:4px;background:black">

<br>

# Application Developer
## [Core Concepts](core-concepts.md#core-concepts)
* [Kubernetes Architecture](core-concepts.md#kubernetes-architecture).
* [Docker vs Container](core-concepts.md#docker-vs-container).
* [Pods](core-concepts.md#pods).
* [Pods with YAML](core-concepts.md#pods-with-yaml).
* [Creating Pods with YAML](core-concepts.md#creating-pods-with-yaml).
* [ReplicaSets](core-concepts.md#replicasets).
* [Deployments](core-concepts.md#deployments).
* [Namespaces](core-concepts.md#namespaces).

<br>

<hr style="height:4px;background:black">

<br>

## [Configuration](core-concepts.md)
* [Define, Build, and Modify Container Images](core-concepts.md#define-build-and-modify-container-images).
* [Commands and Arguments in Docker](core-concepts.md#commands-and-arguments-in-docker).
* [Commands and Arguments in Kubernetes](core-concepts.md#commands-and-arguments-in-kubernetes).
* [Environment Variables](core-concepts.md#environment-variables).
* [Config Maps](core-concepts.md#config-maps).
* [Secrets](core-concepts.md#secrets).
* Demo: [Encrypting Secret Data at Rest](core-concepts.md#demo-encrypting-secret-data-at-rest).
* [Docker Security](core-concepts.md#docker-security).
* [Security Contexts](core-concepts.md#security-contexts).
* [Service Account](core-concepts.md#service-account).
* [Resource Requirements](core-concepts.md#resource-requirements).
* [Taints and Tolerations](core-concepts.md#taints-and-tolerations).
* [Node Selectors](core-concepts.md#node-selectors).
* [Node Affinity](core-concepts.md#node-affinity).
* [Taints and Tolerations vs Node Affinity](core-concepts.md#taints-and-tolerations-vs-node-affinity).

<br>

<hr style="height:4px;background:black">

<br>

## [Multi-Container Pods](core-concepts.md)
* [Multi-Container Pods](core-concepts.md#multi-container-pods).
* Practise Test/Solution: [Creating Multi Container Pods](core-concepts.md#practise-testsolution-creating-multi-container-pods).
* [Init Containers](core-concepts.md#init-containers).
* Practise Test/Solution: [Init Containers](core-concepts.md#practise-testsolution-init-containers).

<br>

<hr style="height:4px;background:black">

<br>

## [Observability](observability.md#observability).
* [Readiness and Liveness Probes](observability.md#readiness-and-liveness-probes).
* [Liveness Probes](observability.md#liveness-probes)
* [Demo: Readiness and Liveness Probes](observability.md#demo-readiness-and-liveness-probes)
* [Container Logging](observability.md#container-logging)
* [Demo: Container Logging](observability.md#demo-container-logging)
* [Monitor and Debug Applications](observability.md#monitor-and-debug-applications)
* [Demo: Monitoring](observability.md#demo-monitoring)

<br>

<hr style="height:4px;background:black">

<br>

## [POD Design](pod-design.md#pod-design)
* [Labels, Selectors and Annotations](pod-design.md#labels-selectors-and-annotations).
* [Demo: Labels, Selectors and Annotations](pod-design.md#demo-labels-selectors-and-annotations).
* [Rolling Updates and Rollbacks in Deployments](pod-design.md#rolling-updates-and-rollbacks-in-deployments).
* [Updating a Deployment](pod-design.md#updating-a-deployment).
* [Deployments: Commands](pod-design.md#deployments-commands).
* [Demo: Rolling Updates](pod-design.md#demo-rolling-updates).
* [Deployment Strategy - Blue green](pod-design.md#deployment-strategy---blue-green).
* [Deployment Strategy - Canary](pod-design.md#deployment-strategy---canary).
* [Demo: Deployment Strategies](pod-design.md#demo-deployment-strategies).
* [Jobs](pod-design.md#jobs).
* [CronJobs](pod-design.md#cronjobs).
* [Demo: Jobs \& CronJobs](pod-design.md#demo-jobs--cronjobs).

<br>

<hr style="height:4px;background:black">

<br>

## [Services & Networking](core-concepts.md#services-and-networking)
* [Services](core-concepts.md#services).
* [Services - Cluster IP](core-concepts.md#services---cluster-ip).
* [Demo: Services](core-concepts.md#demo-services).
* [Ingress Networking](core-concepts.md#ingress-networking).
* [Demo: Ingress Networking (1)](core-concepts.md#demo-ingress-networking-1).
* [Demo: Ingress Networking (2)](core-concepts.md#demo-ingress-networking-2).
* [Network Policies](core-concepts.md#network-policies).
* [Developing Network Policies](core-concepts.md#developing-network-policies).
* [Demo: Network Policies](core-concepts.md#demo-network-policies).

<br>

<hr style="height:4px;background:black">

<br>

## [State Persistence](core-concepts.md#state-persistence)
* [Volumes](core-concepts.md#volumes).
* [Persitent Volumes](core-concepts.md#persitent-volumes).
* [Persistent Volume Claims](core-concepts.md#persistent-volume-claims).
* [Demo: Persistent Volume and Persistent Volume Claims](core-concepts.md#demo-persistent-volume-and-persistent-volume-claims).
* [Storage Classes](core-concepts.md#storage-classes).
* [Why Stateful Sets?](core-concepts.md#why-stateful-sets).
* [Stateful Sets Introduction](core-concepts.md#stateful-sets-introduction).
* [Headless Services](core-concepts.md#headless-services).
* [Storage in Statefulness](core-concepts.md#storage-in-statefulness).

<br>

<hr style="height:4px;background:black">

<br>

## [Security](core-concepts.md#security)
* [Authentication, Autorisation, and Asmission Control](core-concepts.md#authentication-autorisation-and-asmission-control).
* [Authentication](core-concepts.md#authentication).
* [Article on Setting up Basic Authentication](core-concepts.md#article-on-setting-up-basic-authentication).
* [KubeConfig](core-concepts.md#kubeconfig).
* [Demo: KubeConfig](core-concepts.md#demo-kubeconfig).
* [API Groups](core-concepts.md#api-groups).
* [Authorisation](core-concepts.md#authorisation).
* [Role Based Access Controls](core-concepts.md#role-based-access-controls).
* [Demo: Solution Role Based Access Controls](core-concepts.md#demo-solution-role-based-access-controls).
* [Cluster Roles](core-concepts.md#cluster-roles).
* [Demo: Cluster Roles](core-concepts.md#demo-cluster-roles).
* [Admission Controllers](core-concepts.md#admission-controllers).
* [Demo: Admission Controllers](core-concepts.md#demo-admission-controllers).
* [Validating and Mutating Admission Controllers](core-concepts.md#validating-and-mutating-admission-controllers).
* [Demo: Validating and Mutating Admission Controllers](core-concepts.md#demo-validating-and-mutating-admission-controllers).
* [API Versions](core-concepts.md#api-versions).
* [API Deprecations](core-concepts.md#api-deprecations).
* [Demo: API Versions](core-concepts.md#demo-api-versions).
* [Custom Resource Definition](core-concepts.md#custom-resource-definition).
* [Custom Controllers](core-concepts.md#custom-controllers).
* [Operator Framework](core-concepts.md#operator-framework).

<br>

<hr style="height:4px;background:black">

<br>

## [Helm Fundamentals](core-concepts.md#helm-fundamentals)
* [Helm Introduction](core-concepts.md#helm-introduction).
* [Install Helm](core-concepts.md#install-helm).
* [Demo: Install Helm](core-concepts.md#demo-install-helm).
* [Helm Concepts](core-concepts.md#helm-concepts).
* [Demo: Helm Concepts](core-concepts.md#demo-helm-concepts).

<br>

<hr style="height:4px;background:black">

<br>