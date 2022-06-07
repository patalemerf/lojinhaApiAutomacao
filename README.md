# Lojinha API Automação

Esse é um repisitório que contém alguns testes de API Rest de um software denominado Lojinha. Os sub tópicos abaixo descreve algumas decisões tomadas na estruturação do projeto.

## Tecnologias utilizadas

- Java
  https://www.oracle.com/java/technologies/downloads/
-  JUnit
   https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-engine/5.8.0-M1
-  RestAssured
   https://mvnrepository.com/artifact/io.rest-assured/rest-assured/5.1.0
-  Maven
   https://maven.apache.org/

## Testes Automatizados
Testes para validar as partições de equivalência relacionadas ao valor do produto na Lojinha, que estão vinculados diretamente à regra de negócio que diz que o valor do produto deve estar entre R$ 0,01 e R$ 7.000,00.

## Notas Gerais

- Sempre utilizamos a anotação Before Each para capturar o token que   
  será utilizado posterioormente nos métodos de teste.
- Armazenamos os dados que são enviados para a API através do uso de   
  classes POJO.
- Ciramos dados iniciais através do uso de classe    DataFactory   
  para facilitar a criação e controle dos mesmos.
- Nesse projeto fazemos uso do JUnit 5, o que nos dá a possibilidade de
  fazer uso da anotação DisplayName para dar descrição em português dos
  nossos testes.