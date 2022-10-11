# k8s

## kubectl
- kubectl get pods -n $NAMESPACE
- kubectl get pods -n $NAMESPACE --show-labels
- kubectl get pod -n $NAMESPACE $POD -o yaml
- kubectl -n $NAMESPACE logs $POD --all-containers=true --since=5m
- kubectl run -n $NAMESPACE $POD --image=$IMAGE --command -- /bin/bash -c 'while :; do sleep 60; done'
- kubectl apply -f $YAML
  - get from `kubectl get ... -o yaml`
- kubectl exec -it $POD -- /bin/bash
- kubectl delete pod $POD
- kubectl attach $POD -c $CONTAINER -it
- kubectl port-forward $POD $PORT
- kubectl get events
- kubectl auth can-i --list
- kubectl label pods -n $NAMESPACE $POD {foo=bar,name=crazycat}

### cilium
- `kubectl get ciliumnetworkpolicies.cilium.io -n $NAMESPACE $NETWORK_POLICY -o yaml`
- `kubectl delete ciliumnetworkpolicies.cilium.io -n $NAMESPACE $NETWORK_POLICY`
- [Network Policy Editor](https://editor.cilium.io/)
