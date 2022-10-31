# k8s-addons-compatibility
Compatibility details about addons with Kubernetes releases

## Cluster Autoscaler

https://github.com/kubernetes/autoscaler/tree/master/cluster-autoscaler#releases

In cluster autoscaler repo, the helm chart releases are not linked to cluster auto-scaler releases
So we have to fix independantly the helm chart releases and the cluster auto-scaler releases

Example:

- For K8S 1.21 :
  * 9.13.1 is the last chart version that reference the cluster autoscaler version 1.21.x
  * 1.21.3 is the last cluster autoscaler version 1.21.x

- For K8S 1.22 :
  * there are no chart version that reference the cluster autoscaler version 1.22.x so we keep using the 9.13.1
  * 1.22.3 is the last cluster autoscaler version 1.22.x

## Prometheus Operator

https://github.com/prometheus-operator/kube-prometheus#compatibility
https://github.com/prometheus-operator/kube-prometheus/releases

## Istio

https://istio.io/latest/docs/releases/supported-releases/#support-status-of-istio-releases
https://github.com/istio/istio/releases
