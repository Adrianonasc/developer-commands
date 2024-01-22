This command is used to list the running containers
```console
docker ps
```

Para fazer a imagem usamos o comando build e informamos o nome da imagem 'prometheus', a tag e um ponto(.). O comando fica assim: 
docker build -> O comando
-t -> Parâmetro usado para informar que a imagem pertence ao meu usuário
prometheus -> O nome da imagem e a tag atribuída à imagem
. -> significa o diretório atual (pois dei o build dentro da pasta do Dockerfile)
```console
docker build -t prometheus .
```

Para executar testar a imagem vamos criar um contêiner:
```
docker container run -p 9090:9090 prometheus
```
