# buildkite agent

## create namespace
```
kubectl create namespace $NAMESPACE
```

## create secret
```bash
kubectl create secret generic \
        buildkite-agent \
        --from-literal=token=$BUILDKITE_AGENT_TOKEN \
        --namespace=$NAMESPACE
```

## deploy buildkite agent
```
hf apply
```