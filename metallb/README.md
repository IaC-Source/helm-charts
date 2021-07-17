_This is educational purpose chart_ for [metallb](https://github.com/metallb/metallb)

**MetalLB** hooks into your Kubernetes cluster, and provides a network load-balancer implementation. In short, it allows you to create Kubernetes services of type LoadBalancer in clusters that don’t run on a cloud provider, and thus cannot simply hook into paid products to provide load balancers.

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
--set controller.tag=<버전> \
--set speaker.tag=<버전> \
--set configmap.ipRange=<IP 범위> 
```

# Uninstall the Chart
```bash
$ helm uninstall metallb
```
