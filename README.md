# Istio Gateway

A simple chart to manage Istio gateway resources.

#### _This is a mirror of a government repo hosted on [Repo1](https://repo1.dso.mil/) by [DoD Platform One](http://p1.dso.mil/).  Please direct all code changes, issues and comments to https://repo1.dso.mil/platform-one/big-bang/apps/core/istio-gateway_

## Table of Contents

- [Prerequisites](#pre-requisites)
- [Deployment](#deploy-istio-gateway)

## Pre-Requisites

- Kubernetes Cluster deployed
- Kubernetes config installed in `~/.kube/config`
- Helm installed

Install Helm

https://helm.sh/docs/intro/install/

This chart requires the Istio [control-plane](https://repo1.dso.mil/platform-one/big-bang/apps/core/istio-controlplane/-/tree/main)
to be deployed beforehand.  You can use [BigBang]() or the standalone [istio-operator](https://repo1.dso.mil/platform-one/big-bang/apps/core/istio-operator) chart.
Place the chart into the "istio-system" namespace as described below.

## Deployment

```shell
git clone https://repo1.dso.mil/platform-one/big-bang/apps/core/istio-gateway.git
cd istio-gateway
helm install istio-gateway chart -n istio-system
```
