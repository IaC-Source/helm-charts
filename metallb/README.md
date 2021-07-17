_This is educational purpose chart_ for [metallb](https://github.com/metallb/metallb)

**MetalLB** hooks into your Kubernetes cluster, and provides a network load-balancer implementation. In short, it allows you to create Kubernetes services of type LoadBalancer in clusters that don’t run on a cloud provider, and thus cannot simply hook into paid products to provide load balancers.

⚠️ **Caution**: It supports MetalLB version 8 or less. 

# TL;DR
```bash
$ helm repo add edu https://iac-source.github.io/helm-charts
$ helm repo update
```

# Install the Chart
```bash
$ helm install metallb edu/metallb \
--namespace=metallb-system \
--create-namespace \
--set controller.tag=<Version> \
--set speaker.tag=<Version> \
--set configmap.ipRange=<IP Range> 
```

# Uninstall the Chart
```bash
$ helm uninstall metallb
```
