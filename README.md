# statefulset-k8s-example

```sh
kubectl apply -f google_cloud-ssd.yaml
```

```console
storageclass.storage.k8s.io/fast-disk created
```

kubectl apply -f mongo-statefulset.yaml

kubectl get pods

kubectl scale --replicas=4 statefulset mongo

Deletion:

kubectl delete statefulset mongo

kubectl delete svc mongo

kubectl delete pvc -l role=mongo


Troubleshoot:

$ kubectl apply -f mongo-statefulset.yaml

error: error validating "mongo-statefulset.yaml": error validating data: ValidationError(StatefulSet.spec.volumeClaimTemplates[0]): unknown field "annotations" in io.k8s.api.core.v1.PersistentVolumeClaim; if you choose to ignore these errors, turn validation off with --validate=false
