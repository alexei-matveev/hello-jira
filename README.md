#### Experiments with Jira in k3s

Assuming you already installed the Token in your local config:

    $ export KUBECONFIG=~/.kube/config
    $ kubectl get nodes
    $ source <(kubectl completion bash)

Install Jira in Kubernetes

    $ kubectl create namespace hello-jira
    $ kubectl config set-context --current --namespace=hello-jira
    $ kubectl apply -k k3s/

Then visit the [URL](https://jira.localhost).
