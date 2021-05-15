# tekton-demo
Tekton is a cloud native continuous integration and delivery (CI/CD) solution, this is the demo for some simple tests.

## Setup

- Install tekton CLI in MacOS

```
brew tap tektoncd/tools
brew install tektoncd/tools/tektoncd-cli
```
- Deploy all tekton components in k8s cluster

```
auto/deploy-tekton-pipeline-controller
auto/deploy-tekton-triggers-controller
auto/deploy-tekton-dashboard
```

- Forward dashboard in local

```
kubectl -n tekton-pipelines port-forward svc/tekton-dashboard 9097:9097
```

- Deploy task

```
auto/deploy-task
```

- Run task

```
auto/run-task
```

- Run pipeline

```
auto/run-pipeline
```
