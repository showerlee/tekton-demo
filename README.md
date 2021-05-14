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
auto/deploy-tekton
```

- Deploy task

```
auto/deploy-task
```

- Run task

```
auto/run-task
```
