## test lbr 
while true; do curl -s -H "Connection: close" http://backend-service; echo; done

## test svc endpoints
get service endpoint - kubectl get endpoints service-name