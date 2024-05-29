# Flux2 HEAD Repository

This repository provides the initial setup for FluxCD and incorporates additional repositories.

## Prerequisites
- Kubernetes cluster version 1.24 or never

## Bootstrap FluxCD example

```
export GITHUB_TOKEN=<gh-token>
flux bootstrap github \
  --token-auth \
  --owner=brainfair \
  --repository=awesome-flux-head \
  --branch=main \
  --path=clusters/homelab \
  --personal
```

## Additional repositories
- [CRD GitOps repository](https://github.com/brainfair/awesome-flux-crds)
- [Infra GitOps repository](https://github.com/brainfair/awesome-flux-infra)

## Architecture

![High-level design](architecture.drawio.svg)
