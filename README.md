# rotten-potatoes
Projeto desenvolvido durante a iniciativa Kubernetes com Fabricio Veronez

## Criação do cluster com k3d
```sh
$ k3d cluster create meucluster --agents 3 --servers 3 -p "8080:30000@loadbalancer"
```

## Aplicar as configurações do Kubernetes no cluster
Acessar o diretório k8s e executar:
```sh
$ kubectl apply -f deployment.yaml
```

## Comandos úteis
- Listando os pods
    ```sh
    $ kubectl get pods
    ```
- Listando os services
    ```sh
    $ kubectl get services
    ```
- Listando tudo
    ```sh
    $ kubectl get all
    ```
## Configuração
    MONGODB_DB => Nome do database
    MONGODB_HOST => Host do MongoDB
    MONGODB_PORT => Posta de acesso ao MongoDB
    MONGODB_USERNAME => Usuário do MongoDB
    MONGODB_PASSWORD => Senha do MongoDB

## Como acessar
 - Abrir projeto: [localhost:8080](http://localhost:8080)