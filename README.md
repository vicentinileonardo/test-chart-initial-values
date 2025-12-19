

cat <<EOF | kubectl apply -f -
apiVersion: core.krateo.io/v1alpha1
kind: CompositionDefinition
metadata:
  name: test-inital-values
spec:
  chart:
    repo: initalvalues
    url: https://ghcr.io/vicentinileonardo/test-chart-initial-values
    version: 0.1.0
EOF