# Rotten Potatoes
> Repositório dedicado ao Desafio 2 da **Iniciativa Kubernetes**
---
## Instruções

### Clone o repositório
```
git clone https://github.com/darian-beluzzo/rotten-potatoes
cd ./rotten-potatoes
```

### Construa a imagem
```
docker image build -t {usuario_dockerhub}/rotten-potatoes:1.0 .
```

### Faça o push
```
docker push {usuario_dockerhub}/rotten-potatoes:1.0
```

### Crie o cluster com o kind
```
kind create cluster --name meucluster --config cluster.yaml
```

## Faça o deploy no k8s
```
kubectl apply -f k8s/deployment.yaml
```

### Acesse a aplicação pela porta 8080
[http://localhost:8080](http://localhost:8080)
