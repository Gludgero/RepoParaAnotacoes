# Structured Query Language

<hr>

### Menu:

<a href="#Tipos de Dados">- Tipos de Dados</a> <br>
<a href="#Comandos e Cláusulas">- Comandos e Cláusulas</a> <br>
<a href="#Keys">- Keys</a> <br>
<a href="#Operadores Lógicos e Matemáticos">- Operadores Lógicos e Matemáticos</a>
<a href=""></a>
<a href=""></a>

<pre>
          _____                           _______                           _____  
         /\    \                         /::\    \                         /\    \ 
        /::\    \                       /::::\    \                       /::\____\
       /::::\    \                     /::::::\    \                     /:::/    /
      /::::::\    \                   /::::::::\    \                   /:::/    / 
     /:::/\:::\    \                 /:::/~~\:::\    \                 /:::/    /  
    /:::/__\:::\    \               /:::/    \:::\    \               /:::/    /   
    \:::\   \:::\    \             /:::/    / \:::\    \             /:::/    /    
  ___\:::\   \:::\    \           /:::/____/   \:::\____\           /:::/    /     
 /\   \:::\   \:::\    \         |:::|    |     |:::|    |         /:::/    /      
/::\   \:::\   \:::\____\        |:::|____|     |:::|____|        /:::/____/       
\:::\   \:::\   \::/    /         \:::\   _\___/:::/    /         \:::\    \       
 \:::\   \:::\   \/____/           \:::\ |::| /:::/    /           \:::\    \      
  \:::\   \:::\    \                \:::\|::|/:::/    /             \:::\    \     
   \:::\   \:::\____\                \::::::::::/    /               \:::\    \    
    \:::\  /:::/    /                 \::::::::/    /                 \:::\    \   
     \:::\/:::/    /                   \::::::/    /                   \:::\    \  
      \::::::/    /                     \::::/____/                     \:::\    \ 
       \::::/    /                       |::|    |                       \:::\____\
        \::/    /                        |::|____|                        \::/    /
         \/____/                          ~~                               \/____/ 
                                                                                   
</pre>



<h3 id="Tipos de Dados"> Tipos de Dados em uma tabela SQL:
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

<hr>


<h2 id="Comandos e Cláusulas">Comandos e cláusulas (básicos) SQL:</h2>

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

- Drop 
##### O comando drop exclui permanentemente determinado item, sua sintaxe é: DROP tipo_do_objeto nome_do_objeto;
---
- Alter
##### Já o comando alter serve para literalmente, alterar determinada table, coluna, schema, etc... Por exemplo: 

>ALTER TABLE nome_da_tabela
>DROP COLUMN nome_da_coluna;
---
- Insert into / Values
##### Comando para inserir uma linha na tabela existente, se usa o "Insert into nomeTabela (nomeColunas) Values ("x", "y")".

> Uma operação importante é a de combinar o <b>Insert Into</b> com o <b>Select</b>, no lugar do Values, onde podemos inserir dados já existentes de outra tabela no mesmo esquema, e adicionar clausulas como from e where para construir uma Query mais complexa e eficiente.


<hr>

<h2 id="Keys"> Conceito de KEYs

#### Dentro das tabelas SQL é importante a utilização de keys para a manutenção do banco de dados, entre os tipos de chaves temos:

### Primary Key
##### A Chave primária é um indentificador único que desempenha muitas funções em uma table sql, por não poder ser repetida, é um ótimo indentificador facilitando pesquisas e aumentando a eficiência dos sgdbs por serem automaticamente indexadas por eles, além de atuarem na preservação da integridade dos dados.
---
### Foreign Key
##### Uma "Chave Estrangeira" serve para, principalmente, relacionar duas tabelas, sendo muito importante na análise de dados 


---

<h3 id="Operadores Lógicos e Matemáticos">Operadores Lógicos e Matemáticos:</h3>

<p> A Sintaxe SQL não difere muito do padrão para operdadores lógicos, sendo >, <, maior e menor que, = igual >=, <=, maior e menor ou igual também são iguais apenas o sinal de <b>"Diferente de"</b> que é representado pelo sinal de "<>".</p>

<p> Mas uma característica importante é que os operadores matemáticos não são exclusivos dos números, podemos usar, por exemplo, "WHERE nomeColuna > C", para serem selecionados apenas nomes que comecem com as letras que vem depois de C no alfabeto, essa lógica também se aplica pra datas e horas.
