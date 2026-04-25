external dns name mapped to a service - provides a DNS alias to an external service, allowing internal clients to use a stable name without changing application code

spec:
type: ExternalName
externalName: my.api.example.com

kubectl run curl-pod \
 --image=curlimages/curl \
 -it --rm -- sh

curl http://ext-nm/
