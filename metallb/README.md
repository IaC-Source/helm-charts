[metallb](https://github.com/metallb/metallb) is an open source, rock solid LoadBalancer. It handles the ServiceType: Loadbalancer.

_this is education purpose chart_

# TL;DR
```bash
$ helm repo add metallb https://iac-source.github.io/helm-charts
$ helm install metallb --create-namespace --namespace=metallb-system edu/metallb
```

# Install the Chart
```bash
$ helm repo add metallb https://iac-source.github.io/helm-charts
$ helm install metallb --create-namespace --namespace=metallb-system edu/metallb
```

# Install MetalLB with security mode (+ v9.0.3 )
```bash

$ kubectl create ns metallb-system
$ kubectl create secret generic -n metallb-system memberlist --from-literal=secretkey="$(openssl rand -base64 128)"
$ helm install metallb metallb/metallb \
--namespace=metallb-system \
--set controller.tag=v0.9.3 \
--set speaker.tag=v0.9.3 \
--set configmap.ipRange=192.168.1.11-192.168.1.29 \
--set security.enabled=true 
```

# Uninstall the Chart
```bash
$ helm uninstall metallb
```
