
#### Arquivos de migration:
Guardam o versionamento do esquema do Banco de Dados. Eles representam mudanças na estrutura do banco de dados. Criar uma nova tabela, alterar uma tabela, instalar drivers e inserir dados default em massa são exemplos de mudanças na estrutura de um banco de dados.
Nesses arquivos temos um registro de tudo que foi executado no banco.

Os arquivos de migration devem seguir um padrão de nomenclatura para serem processados corretamente pelo Flyway: `VERSAO__nome`. Por exemplo, `V1__create-table.sql`.
Antes de criar um arquivo de migration, é necessário interromper a execução da aplicação.
Toda vez que a aplicação inicializar, o Flyway vai procurar os arquivos de migration, executar (se já não tiver sido executado), e salvar no banco.


#### Entidades
Classes que representam as entradas de dados da tabela.

#### Record
Representa objetos que não são alterados uma vez que foram criados

#### Banco de dados em memória
Toda vez que a aplicação é reiniciada, todas as informações do banco se perdem

#### Mais informações
Spring Initializr: Java 21, Maven, Spring Boot 3.3.1
