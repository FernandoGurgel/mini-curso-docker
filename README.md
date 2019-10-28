Baixando imagem ubuntu

```shell
$ docker pull ubuntu
```

Execultando um container

```shell
$ docker run -it --name appA ubuntu
```

Criar pasta minicurso
```shell
$ mkdir minicurso
```

Atualizando repositorio linux
```shell
$ apt update
```

Instalando curl
```shell
$ apt install curl
```

Instalando nodejs
```shell
$ curl -fsSL https://raw.githubusercontent.com/zeit/install-node/master/install.sh -o install-node.sh | chmod +x install-node.sh | ./install-node.sh -y
```

Criando nossa pasta do mini curso
```shell
$ mkdir minicurso
$ cd minicurso
```

Salva meu container
```shell
$ docker commit appA minicurso:test
```

Apaga um container
```shell
$ docker rm appA
```

Apaga um container
```shell
$ docker rm appA
```

Rodando container com volume e porta
```shell
$ docker run -it --name appA -p3000:3000 -v $(pwd)/minicurso:/minicurso minicurso:test
```

Iniciando Expressjs
```shell
$ npm init -y
$ npm i express
```

Iniciar container

```shell
$ docker start -i appA 
```

Criar rede load balance
```shell
$ docker pull nginx
$ docker run --name load -v $(pwd)/config/nginx.conf:/etc/nginx/nginx.conf -p80:80 -d nginx 
```





