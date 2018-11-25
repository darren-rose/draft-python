# draft python

Example using draft to provision a python app into a Kubernetes cluster

1. draft create
* Optional: change the namespace, type, etc in draft.toml:
```
namespace = "my-namespace"
set = ["service.type=NodePort", "service.externalPort=30000"]
```
1. draft up
1. kubectl get pods --all-namespaces | grep draft-python
1. draft connect
1. curl localhost:XXXXX
