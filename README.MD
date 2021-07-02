# Uma aplicação conteineirizada escrita em Python e orquestrada via Kubernetes

Este repositório trata de um projeto cuja aplicação escrita em python está conteineirizada e é orquestrada via kubernetes.

Para executar esta aplicação tenha um cluster local ou remoto, faça o clone deste repositório e execute os seguintes comandos:

```bash
$ cd rottenpotatoes
$ kubectl apply -f .\k8s\monbodb\deployment.yaml
$ kubectl apply -f .\k8s\web\deployment.yaml
```

Após executar os comandos sua aplicação poderá ser acessada através do navegador de internet com o endereço: `localhost:8080`

![](C:\Users\thiag\Dropbox\PROJETOS\Kubernetes Bootcamp\Aula 02 - Kubernetes\rotten-potatoes\01.png)

Para finalizar:

```bash
$ kubectl delete -f .\k8s\monbodb\deployment.yaml
$ kubectl delete -f .\k8s\web\deployment.yaml
```



See ya...