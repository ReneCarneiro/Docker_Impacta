Olá Professor João Henrique.

Segues os comandos conforme pedido em sala de aula.

1-Baixar as imagens necessárias para a criação dos containers de mysql e nginx.

docker pull nginx

docker pull mysql

2 - Agora vamos executar o primeiro container para mysql:

docker run -d --name mysql-docker-container -e MYSQL_ROOT_PASSWORD=docker1234 mysql

para testar o container acima, exeutando o comando abaixo, caso tudo esteja correto a uma mensagem relacionada ao mysql será exibida

docker exec -it mysql-docker-container mysql -p 

3 - Agora iremos executar o container do nginx conforme abaixo:

docker run -d --name nginx-container -p 80:80 nginx

4 - Para listar os container criados digite o comando abaixo:

docker ps
