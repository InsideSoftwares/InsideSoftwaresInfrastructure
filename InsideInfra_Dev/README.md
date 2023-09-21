# Infraestrutura de Desenvolvimento

## Será necessarios os seguintes projetos buildados na sua maquina:
  * [InsideSoftwaresCloudConfig](https://github.com/InsideSoftwares/InsideSoftwaresCloudConfig)
  * [InsideSoftwaresCloudAdmin](https://github.com/InsideSoftwares/InsideSoftwaresCloudAdmin)
  * [InsideSoftwaresCloudGateway](https://github.com/InsideSoftwares/InsideSoftwaresCloudGateway)

## Possui 5 docker-compose sendo:
  * [docker-compose-database_mysql](docker-compose-database_mysql.yml)
    * Cria uma base Mysql 8.1 ou superior
  * [docker-compose-database_postgresql](docker-compose-database_postgresql.yml)
    * Cria uma base Postgres 15 ou superior
  * [docker-compose-keycloak](docker-compose-keycloak.yml)
    * Cria um Keycloak em modo desenvolvimento, onde e importado os dados da pasta `./keycloak`
  * [docker-compose-database_redis](docker-compose-database_redis.yml)
    * Cria uma base de Redis no modo Sentinel (Utilizado para Cache e Idempotência)
  * [docker-compose](docker-compose.yml)
    * Cria os container dos sistemas necessarios para realizar os desenvolvimento e teste da estrutura

## Estrutura das pastas
  * keycloak
    * Contém as configurações necessárias para utilização do Keycloak
  * logs
    * Onde será escritos os logs dos containers em execução
  * properties 
    * Contém os properties dos sistemas