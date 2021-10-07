# Prometheus-operator
## Requirements
1. Install [Prometheus-operator](https://github.com/prometheus-operator/prometheus-operator)

## Example
1. Create namespace
```shell
kubectl apply -f namespace.yml
```
2. Start apps
```shell
kubectl apply -f app-one.yml
kubectl apply -f app-two.yml
```
3. Create prometheus-operator for app's namespace
```shell
kubectl apply -f operator.yml
```
4. Create ClusterRole for prometheus and start Prometheus
```shell
kubectl apply -f rbac.yml
kubectl apply -f prometheus.yml
```