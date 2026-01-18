# metadata 

```yaml
metadata:
    name: nginx-static-name
    generateName: nginx-pod-dynamic # use create not apply
    namespace: default
    annotations:
        description: "My 1st pod ever" # use describe cmd to see the affect
    labels:
        k: v
```

1. `kubectl get objects --show-labels` → gives us all the pods with their pod labels 
2. `kubectl get pods --show-labels`
3. `kubectl get pods pod-name --show-labels`


# selectors 

