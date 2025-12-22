# ArgoCD Demo

This repo consists of the ArgoCD Config file and sample K8s yaml files that we will use to test our ArgoCD solution.
We will use these files to setup our ArgoCD Operator and test deployment to our K8s cluster using the sample K8s yaml files.

application.yaml is the main config file for ArgoCD, it will refer to it whenever it needs to make changes such a:
repos/environments.

We will test out deployments (dev/prod) in different environments/teams.

The docker images used by our docker pull are found at https://hub.docker.com/repository/docker/zulqadara/argocd-demo/

Fell free to pull these images to test your pipeline/demo.


P.s. Dont forget to make your namespace:
*# kubectl create ns dev*
*# kubectl create ns prod*

Also to apply the main application.yaml file
*#  kubectl apply -f <path-to-folder/application.yaml>*