Apply Updated CRDs for Version 0.49

Note: It works for both: create and update CRDs.
Initially CRDs are part of Operator installation.

Important: Apply the new CRDs before upgrading the operator:

``` bash
kubectl apply -f https://github.com/strimzi/strimzi-kafka-operator/releases/download/0.49.1/strimzi-crds-0.49.1.yaml
```

Reference: https://github.com/strimzi/strimzi-kafka-operator/blob/main/packaging/helm-charts/helm3/strimzi-kafka-operator/README.md#upgrading-your-clusters
