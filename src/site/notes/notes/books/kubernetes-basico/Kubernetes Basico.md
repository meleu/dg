---
{"dg-publish":true,"permalink":"/notes/books/kubernetes-basico/kubernetes-basico/","dgHomeLink":true,"dgPassFrontmatter":false}
---

# livro: Kubernetes Básico

- [[notes/books/kubernetes-basico/01-introducao|01-introducao]]
- [[notes/books/kubernetes-basico/02-containers|02-containers]]
- [[notes/books/kubernetes-basico/03-cluster-kubernetes|03-cluster-kubernetes]]
- [[notes/books/kubernetes-basico/04-kubectl|04-kubectl]]
- [[notes/books/kubernetes-basico/05-pods|05-pods]]
- [[notes/books/kubernetes-basico/06-labels-annotations|06-labels-annotations]]


## Capítulo 7: Descoberta de serviços

Os exemplos do livro (p. 102) não funcionam exatemente daquela forma pois `kubectl run` não é mais usado para criar deployments.

Mas adaptando, dŕa pra fazermos o seguinte para criar um Service do tipo `ClusterIP`:

```sh
# criando o deployment
kubectl create deployment alpaca-prod \
  --image=gcr.io/kuar-demo/kuard-amd64:blue \
  --replicas=3 \
  --port=8080

# expondo o deployment (equivale a criar um ClusterIP)
kubectl expose deployment alpaca-prod

# criando outro deployment
kubectl create deployment bandicoot-prod \
  --image=gcr.io/kuar-demo/kuard-amd64:green \
  --replicas= 2 \
  --port=8080

# expondo
kubectl expose deployment bandicoot-prod

# ver os selectors
kubectl get services -o wide

# encaminhamento de portas para acessar o app
ALPACA_POD="$(kubectl get pods -l app=alpaca-prod \
  -o jsonpath='{.items[0].metadata.name}')"
kubectl port-forward "${ALPACA_POD}" 48858:8080

launch http://localhost:48858
```

### demonstração do `readinessProbe`

```sh

```


