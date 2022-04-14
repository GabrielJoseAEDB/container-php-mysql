# container-php-mysql
Repositório para imagem docker que conterá uma versão do php 7.2, com as extensões necessárias pelo moodle 3.5

Instruções:
-Instalar docker e docker-compose  
-Baixar este repositório através de git clone ou zip  
-Executar (sudo )docker-compose up -d na pasta  
-Aguardar a execução do script  
-Utilizar os dados contidos em docker-compose.yml para configurar a nova instalação  
  
Observações:  
-O host do banco a ser usado é o nome do container mysql, no caso: mysqlASW  
-No arquivo dockerfile é possível alterar a versão da imagem do php e também a tag do moodle, caso almeje outra versão  
-A pasta www pode ser usada para pre-montar arquivos dentro de /var/www  
-a pasta mysql-dump pode ser usada para pré-executar scripts de restore de banco na primeira iniciação  
###### https://stackoverflow.com/questions/36617682/docker-compose-mysql-import-sql