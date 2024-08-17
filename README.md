# Desafios - Docker Primeiros Passos

<details><summary>Desafio 01 - Banco de Dados Postgresql</summary>

Você está dando os primeiros passos no uso de containers. E a melhor forma de iniciar no mundo de containers é usar em ambiente de desenvolvimento.

Sua missão é ajudar a equipe de desenvolvimento a ter mais autonomia no desenvolvimento de projetos. E uma das reclamações da equipe é o setup local.

Crie um comando para criar um banco de dados PostgreSQL no ambiente do desenvolvedor de uma forma que cumpra os seguintes requisitos:
* O nome do banco de dados deve ser curso_docker
* O usuário de acesso ao banco deve ser docker_usr
* A senha do usuário deve ser docker_pwd

Lembrando que a execução em container deve ser transparente pra quem está desenvolvendo. E que aqui você não precisa se preocupar com a perda dos dados do banco e nem nada disso, é apenas para desenvolvimento pontual.
Coloque aqui embaixo o comando que a equipe deve usar pra criar um banco de dados PostgreSQL com esses requisitos.

# Solução

[Postgres - Official Image | Docker Hub](https://hub.docker.com/_/postgres)

```sh
$ docker container run -d -p 5432:5432 -e POSTGRES_DB="curso_docker" -e POSTGRES_USER="docker_usr" -e POSTGRES_PASSWORD="docker_pwd" p
ostgres

Unable to find image 'postgres:latest' locally
latest: Pulling from library/postgres
e4fff0779e6d: Already exists
3dd23fa89c28: Pull complete
9110f5284332: Pull complete
b2a5b191a941: Pull complete
f0baaf1c42c6: Pull complete
3c42bd6bf488: Pull complete
cb55f9f5ebf8: Pull complete
6eeec50ef8e1: Pull complete
ba3d1f8aa002: Pull complete
199cdf05dfec: Pull complete
438d147df750: Pull complete
a2e706f2e593: Pull complete
2505d0b60422: Pull complete
133de8acf4aa: Pull complete
Digest: sha256:c62fdb7fd6f519ef425c54760894c74e8d0cb04fbf4f7d3d79aafd86bae24edd
Status: Downloaded newer image for postgres:latest
9b28d31730a0bfae9ec5944e80b40675cc9c3c513c94c21b7d2ef164066b0aa5
```

[Download DBeaver Community](https://dbeaver.io/download/)

![image](https://github.com/user-attachments/assets/55c80380-c284-4e6a-9122-74203a8a23c6)

![image](https://github.com/user-attachments/assets/0e6decc9-7e20-4050-9469-4e8aa3ed516f)

</details>
