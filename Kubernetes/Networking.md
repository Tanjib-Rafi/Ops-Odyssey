- CoreDNS   → Finds service IP
- CNI       → Connects pods/network
- kube-proxy→ Sends traffic to pods
- Envoy     → Smart traffic proxy
- Istio     → Controls Envoy

look for CNI daemonset
```kubectl get ds -n kube-system kube-proxy```
