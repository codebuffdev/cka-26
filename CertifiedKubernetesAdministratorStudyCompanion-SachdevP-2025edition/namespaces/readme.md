kubectl create namespace nm
kubectl get ns
kubectl get pod -n ns
kubectl run pod --image=img -n ns
kubectl create deploy nginx-deploy --image=nginx --replicas=4 -n poc2

kubectl delete deploy/nginx-deploy -n poc2
deployment.apps "nginx-deploy" deleted

kubectl get all -n poc2

## diff obj in diff ns communication

# svcName.namespace.svc.cluster.local
