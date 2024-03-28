# Jenkins
[Jenkins](https://www.jenkins.io/) is an open source automation server. It helps automate the parts of software development related to building, testing, and deploying, facilitating continuous integration, and continuous delivery
## Installation
```console
helm repo add jenkinsci https://charts.jenkins.io
helm repo update
helm search repo jenkinsci
kubectl apply -f jenkins-volume.yaml
kubectl apply -f jenkins-sa.yaml

edit jenkins-value.yaml
serviceAccount:
  create: false
name: jenkins

helm install --values jenkins-values.yaml jenkins jenkinsci/jenkins --namespace jenkins
```