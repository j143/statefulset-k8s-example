# statefulset-k8s-example

kubectl apply -f google_cloud-ssd.yaml

kubectl apply -f mongo-statefulset.yaml

kubectl get pods

kubectl scale --replicas=4 statefulset mongo

Deletion:

kubectl delete statefulset mongo

kubectl delete svc mongo

kubectl delete pvc -l role=mongo
