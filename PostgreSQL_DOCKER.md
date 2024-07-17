# Passo a passo para rodar PostgreSQL em um container Docker

## 1. Baixe a imagem do PostgreSQL

Abra o terminal e digite:

```
docker pull postgres
```

Este comando irá baixar a última versão do PostgreSQL da base de dados do Docker.

## 2. Crie o container

Execute o comando abaixo no terminal:

```
docker run -d --name postgres-db -p 5432:5432 -e POSTGRES_PASSWORD=root postgres
```

Neste comando, estamos pedindo ao Docker para:

- -d: Executar o container em modo "detached" (em segundo plano, não trava o terminal).
- --name: Nomear o container como postgres-db.
- -p 5432:5432: Mapear a porta 5432 do container para a porta 5432 da máquina host.
- -e POSTGRES_PASSWORD=root Definir a senha do usuário padrão postgres.
- postgres: Especificar a imagem do Docker a ser usada.

## 3. Iniciar e Parar o container

Para iniciar o container, digite no terminal:

```
docker start postgres-db
```

Para parar o container, digite no terminal:

```
docker stop postgres-db
```
