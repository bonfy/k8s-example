# k8s-example
k8s example


```cmd
# LoadBalancer

$ kubectl apply -f .\service.yaml
$ kubectl get pods
NAME                            READY   STATUS    RESTARTS   AGE
hello-python-6f7d964c75-mrpm8   2/2     Running   0          2s
hello-python-6f7d964c75-nsgps   2/2     Running   0          2s

$ kubectl port-forward service/hello-python-service 7000:6000 
$ kubectl delete -f .\service.yaml


# NodePort
$ kubectl apply -f .\service.yaml
$ kubectl get pods
NAME                            READY   STATUS    RESTARTS   AGE
hello-python-6f7d964c75-mrpm8   2/2     Running   0          2s
hello-python-6f7d964c75-nsgps   2/2     Running   0          2s
$ kubectl delete -f .\service.yaml

```