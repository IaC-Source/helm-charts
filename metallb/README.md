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

# Uninstall the Chart
```bash
$ helm uninstall metallb
```
