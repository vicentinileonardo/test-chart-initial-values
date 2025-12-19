
```sh
cat <<EOF | kubectl apply -f -
apiVersion: core.krateo.io/v1alpha1
kind: CompositionDefinition
metadata:
  name: test-inital-values
spec:
  chart:
    url: oci://ghcr.io/vicentinileonardo/test-chart-initial-values/initialvalues
    version: 0.1.1
EOF
```