## Helm charts for Hyperledger Fabric

Add the helm repository to your helm client:
```bash
helm repo add kfs https://kfsoftware.github.io/hlf-helm-charts --force-update 
```

Default values can be found in [charts/hlf-operator/values.yaml](values.yaml)


### Installing hlf-operator

With default values:
```bash
helm install hlf-operator --version=1.6.0 kfs/hlf-operator
```

With custom values:
```bash
helm install hlf-operator -f values.yaml --version=1.6.0 kfs/hlf-operator
```
