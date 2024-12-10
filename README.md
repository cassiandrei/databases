# Setup de serviços usados

## antes de usar:

- verificar .env e alterar o nome de usuário;
- criar uma network docker chamada serviços `docker network create servicos`;

## comandos postgres direto no terminal host:

para atalhar seus comandos básicos do postgres como `psql`,`pg_restore`,`createdb` entre outros...
será necessário duas coisas:

- instalar os comandos(se já não tiver instalado):
  pode fazer isso do jeito mais fácil instalando um cliente postgres e deixando adormecido
  ou pode instalar(se disponível pro seu sistema) a libpq-dev
- adicionar duas constantes no seu `.bashrc` ou `.zshrc`:
  ```bash
  export PGHOST="localhost"
  export PGUSER="<usuário que você colocou lá no .env>"
  ```
