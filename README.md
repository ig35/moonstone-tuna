# moonstone-tuna

[![Validate ingress](https://github.com/ig35/moonstone-tuna/actions/workflows/minikube.yaml/badge.svg)](https://github.com/ig35/moonstone-tuna/actions/workflows/minikube.yaml)

Enforce ingress policy using Open Policy Agent.

## Problem Statement

We use namespace isolation to allow engineering teams to share Kubernetes
resources safely. But DNS is global so we need to put guardrails in place so
that no two services can use the same ingress hostname. How can we enforce that
within the cluster?
