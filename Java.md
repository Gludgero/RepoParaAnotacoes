# Java

<h2> Index :</h2> 


<a href=#OperadoresLógicos> - Operadores Lógicos <br></a>

<a href=#Convenções> - Convenções e Boas práticas  <br></a>

<a href=#Casting> - Casting  <br></a>


---

<pre>
______/\\\\\\\\\\\_______________/\\\\\\\\\_______________/\\\________/\\\_______________/\\\\\\\\\____        
 _____\/////\\\///______________/\\\\\\\\\\\\\____________\/\\\_______\/\\\_____________/\\\\\\\\\\\\\__       
  _________\/\\\________________/\\\/////////\\\___________\//\\\______/\\\_____________/\\\/////////\\\_      
   _________\/\\\_______________\/\\\_______\/\\\____________\//\\\____/\\\_____________\/\\\_______\/\\\_     
    _________\/\\\_______________\/\\\\\\\\\\\\\\\_____________\//\\\__/\\\______________\/\\\\\\\\\\\\\\\_    
     _________\/\\\_______________\/\\\/////////\\\______________\//\\\/\\\_______________\/\\\/////////\\\_   
      __/\\\___\/\\\_______________\/\\\_______\/\\\_______________\//\\\\\________________\/\\\_______\/\\\_  
       _\//\\\\\\\\\________________\/\\\_______\/\\\________________\//\\\_________________\/\\\_______\/\\\_ 
        __\/////////_________________\///________\///__________________\///__________________\///________\///__
</pre>

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

---
<h3 id="OperadoresLógicos"> Operadores Lógicos </h3>

---
<p> Assim como na maioria das linguagens, no java temos operadores lógicos para declarar condições de forma mais eficiente. </p>

> Temos: "AND" (&&), "OR" (||) e "NOT" (!)

---

<br>
<br>
<br>

---

<h3 id="Convenções">Convenções e Boas práticas </h3>

<pre>
- Nomes de classes devem começar com letra maiúscula e usar a convenção PascalCase.

- Nomes de métodos devem começar com letra minúscula e usar a convenção camelCase.

- Nomes de constantes devem ser totalmente em letras maiúsculas, separadas por underline.

- Nomes de variáveis devem usar a convenção camelCase.

- Recomenda-se usar espaços em branco para separar operadores, palavras-chave e elementos de controle de fluxo. 

    Exemplo: if (condicao) {...
</pre>

---

<br>
<br>
<br>

---

<h3 id="Casting">Casting dentro Do Java</h3>

Dentro do Java, uma linguagem de tipagem forte, podemos converter variáveis, alterando seu tipo atraves do casting <b>Implicito ou Explicito </b>.

Basta se basear na imagem abaixo para saber o tipo de casting, uma vez que o tipo antigo seja menor que o novo, usa-se apenas a atribuição básica para o valor, como em:
> x = ...;

Mas caso a nova "casa" do valor seja menor que a "casa antiga" um double se convertendo para int, por exemplo, precisamos <b> Explicitá-lo </b>usando o (casa nova), como em: 
>int y = (int) x;

---

A tabela abaixo serve para a consulta da compatibilidade das conversões.

---
![alt text](image.png)

---
<br>
<br>
<br>

---

