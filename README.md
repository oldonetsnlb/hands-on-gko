# 🧪 Kubernetes Operator Hands On

![Gravitee.io](./.assets/gravitee-logo-cyan.svg)


## 📼 Foreword

This repository is aimed at adding Custom Resources handled by the Gravitee Kubernetes Operator.
Some basic examples have already been prepared for each supported resources in the `resources` directory.
To make things simpler, a CircleCI pipeline will handle deploying resources in a dedicated namespace on a demo cluster.


## 👷‍♀️ Workflow

  - ➡️ Fork this repository
  - ⬇️ Clone your fork
  - 🔄 Add / Modify custom resources in the `resources` directory
  - ⬆️ Update your fork
  - ⬅️ Submit your pull request to this repository
  - 🔄 The Circle CI pipeline will deploy resources on your behalf when your pull request is merged.

⚠️ On merge, the pipeline will apply all resources in the `resources` folder on a dedicated namespace (namely `gko-hands-on`). As a consequence your custom resource **should not reference a namespace**.

## 🌡 Limitations

As the workflow is built around a simple kubectl command that will recursively apply all resources in the `resources` directory, it does not handle resources deletion.
