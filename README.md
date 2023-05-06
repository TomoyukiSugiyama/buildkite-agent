# buildkite agent

```
kubectl create namespace $NAMESPACE
```

```bash
kubectl create secret generic \
        buildkite-agent \
        --from-literal=token=$BUILDKITE_AGENT_TOKEN \
        --namespace=$NAMESPACE
```