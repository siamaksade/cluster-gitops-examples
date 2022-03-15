# BU Cluster Examples

## Directories

* `clusters/hub`: RHACM and OpenShift Hub cluster configurations
* `clusters/all`: all spoke cluster configurations
* `clusters/dev`: dev cluster configuration overrides
* `clusters/prod`: prod cluster configuration overrides


## Setup

1. Install OpenShift GitOps on the Hub cluster from the OperatorHub

2. Navigate to the Cluster Argo CD from the Red Hat Application menu, or from the `openshift-gitops` namespace

3. Create [`hub-argocd-rolebinding.yaml`](hub-argocd-rolebinding.yaml) on the Hub cluster in order to elevate Argo CD privileges to be able to managed RHACM configurations:

4. Create [`hub-application.yaml`](hub-application.yaml) on the Hub cluster