# Full removal

``` bash
helm uninstall kafka-deployment -n kafka

helm uninstall strimzi-kafka-operator -n kafka

kubectl delete pvc -n kafka --all

kubectl get pv -o json | jq -r '.items[] | select(.spec.claimRef.namespace=="kafka") | .metadata.name' | xargs kubectl delete pv

kubectl get crd | grep strimzi.io | awk '{print $1}' | xargs kubectl delete crd
```
