# Passo a passo para rodar MySQL em um container Docker

* Primerio abra o terminal e digite:
	* `docker pull mysql`
	* no comando acima ele irá baixar da base de dados do docker a última versão do MySQL.

* Depois vamos rodar no terminal outro comando
	* `docker run -d --name mysql-db -p 3306:3306 -e "MYSQL_ROOT_PASSWORD=root" mysql`
	* nesse comando pedimos ao Docker para criar um conteiner nomeando ele para *mysql-db*, depois específico a porta de acesso ao container, depois defino uma senha de acesso ao database e por útlimo digo qual a imagem que o container irá rodar como base.



