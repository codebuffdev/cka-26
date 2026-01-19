# cka-26
Going through k8s core concepts for the CKA26. 

## pod
### imperative 
    kubectl run nginx --image=nginx -l app=fe 

## metadata
### labels
#### Imperative
add label to an existing object : kubectl label object object-name -l labelK=labelV
#### Declarative 
```yaml
apiVersion: v1
kind: Pod
metadata:
  name: my-pod
  labels:
    app: my-app
```  
### selectors 
#### Imperative
#### Declarative
