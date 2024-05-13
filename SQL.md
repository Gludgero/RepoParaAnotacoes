# Structured Query Language

### Comandos e cláusulas (básicos) SQL:

#### "*" 
##### Equivalente à "todos"
<hr>

- From 
##### Cláusula para especificar de qual tabela queremos buscar
<hr>

- Select 
##### Literalmente seleciona, e exibe determinado dado
<hr>

- Where 
##### O Where serve para definir uma condição específica, como: 
SELECT * FROM tabelaX WHERE nomeColuna = '50';
<hr>

##### Esse comando trará todos as linhas que contenham o valor 50 na coluna especificada. 
#### Atenção, a string tem que estar entre aspas simples (pelo menos no sqlite)
<hr>

- Select Distinct 
##### Garante que X coluna não será exibida mais de uma vez

<hr>

- Creat Table
##### Cria tabela, exemplo:

CREATE TABLE tabelaClientes (
    ID iNT PRIMARY KEY, 
    nomeCliente varchar (250),
    infosDeCadastro varchar (250),
);

##### Esse comando cria uma tabela chamada tabelaClientes, com três colunas a primeira sendo chamada de ID, sendo declarada do tipo inteiro e como a chave primária da tabela, as outras duas são do tipo VARCHAR e tem o limite de caracteres definido em 250.

<hr>

### Tipos de Dados em uma tabela SQL:
<hr>

#### Strings:

- Char 
##### Armazena strings de tamanho constante

- VarChar 
##### Armazena strings de tamanho variável

- Text 
##### Armazena strings muito longas

<hr>

#### Numéricas: 

- int 
##### Armazena números inteiros

- Float
##### Armazena números com ponto flutuante

- Numeric 
##### Armazena precisamente números decimais

<hr>

#### Data e hora: 

- Date
##### Armazena somente data

- Time
##### Armazena somente horas

- TimeStamp
##### Armazena ambos em um único dado

<hr>

- Booleano
##### Armazena flags de verdadeiro ou falso

- BLOB
##### Armazena dados binários, como imagens ou arquivos.


