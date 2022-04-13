# Atividade: AC2

### Ctrl + Insert = copiar;

### Shift + Insert = colar;

### Alt + Enter = maximizar o ambiente;

### * Obtendo Imagem de MySQL:

### docker pull mysql:5.7 - comando que permite baixar o banco de dados;

### docker pull mysql:latest - comando que permite baixar ultima versao;

### docker run --name mysql5 -e MYSQL_ROOT_PASSWORD=mudar123 -p 3307:3307 -d mysql:5.7 - comando para subir o container;

### hash: b98e08bbed270adecb1b84890eabc63a81973aef75d19c65681b25dbec98e8b8

### docker ps - comando para visualizar quantos containers estao sendo executados;

### docker network inspect bridge - comando para visualizar IP da aplicacao;

### docker exec -it b98e08bbed27 /bin/bash - comando para acessar o container;

### mysql -uroot -p - comando para acessar o mysql;

### show schemas; - comando para visualizar quais schema/database estao ativos no mysql;

### create schema teste; - comando para criar um novo schema/database;

### use teste; - comando para selecionar o schema/database;

### show tables; - comando para visualizar tabelas criadas no schema/database;

### CREATE TABLE tbl_user (

### 	user_id BIGINT NOT NULL AUTO_INCREMENT, 

### 	user_name VARCHAR(45) NULL, 

### 	user_username VARCHAR(45) NULL, 

### 	user_password VARCHAR(45) NULL, 

### 	PRIMARY KEY (user_id)

### ); - criacao de tabela

### desc tbl_user; - comando para mostrar informacoes da tabela;

### exit - comando para sair do ambiente que estiver;

## * Conectando database com aplicacao

### ls - comando para visualizar pastas e arquivos do ambiente;

### ls -lts - comando para visualizar pastas e arquivos do ambiente de forma organizada;

### pwd - comando para visualizar pasta atual;

### git clone https://github.com/antoniodiasabc/docker2.git - comando para clonar repositorio;

### vi Dockerfile - comando para acessar arquivos;

### Esc + :wq - comando para salvar e sair do arquivo acessado;

### Esc + i - comando para permitir edicao de arquivo;

### python3 app3.py - comando para executar aplicacao web;

### docker image build -t python_web . - criacao de imagem baseado em dockerfile

### docker image ls - elencar as imagens construidas

### docker run python_web -d - sobe container baseado na imagem criada

### docker run -p 5000:5000 -d python_web - define porta em que a app sera executada

### docker run --link mysql5:mysql5 -p 5000:5000 -d python_web - associa com o banco de dados criado

![alt text](https://github.com/lucianonevesln/ac2_docker/blob/main/img0.png)

![alt text](https://github.com/lucianonevesln/ac2_docker/blob/main/img1.png)

![alt text](https://github.com/lucianonevesln/ac2_docker/blob/main/img2.png)

![alt text](https://github.com/lucianonevesln/ac2_docker/blob/main/img3.png)

![alt text](https://github.com/lucianonevesln/ac2_docker/blob/main/img4.png)

![alt text](https://github.com/lucianonevesln/ac2_docker/blob/main/img5.png)
