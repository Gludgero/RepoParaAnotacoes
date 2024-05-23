## Estruturas de Dados
<p>Bem vindo novamente! Por aqui vou classificar algumas coisas e anotar algumas caracteríscias das principais estruturas de dados, alguns exemplos também, relembrando, esse MD não tem a intenção de ensinar nada para ninguém, sua única função é registrar minhas anotações e me ajudar a sintetizar meus tópicos estudados.</p>

---

### Index: 

<a href="#Arrays">- Arrays</a> <br>
<a href="#Listas Encadeadas">- Listas Encadeadas</a> <br>


---

<pre>


  _____        _           _____ _                   _                       
 |  __ \      | |         / ____| |                 | |                      
 | |  | | __ _| |_ __ _  | (___ | |_ _ __ _   _  ___| |_ _   _ _ __ ___  ___ 
 | |  | |/ _` | __/ _` |  \___ \| __| '__| | | |/ __| __| | | | '__/ _ \/ __|
 | |__| | (_| | || (_| |  ____) | |_| |  | |_| | (__| |_| |_| | | |  __/\__ \
 |_____/ \__,_|\__\__,_| |_____/ \__|_|   \__,_|\___|\__|\__,_|_|  \___||___/
                                                                             
                                                                             
</pre>

---

<h4 id="Arrays"> Arrays .. </h4>
<p>Basicamente um conjunto de dados, primitivos ou não, diferentes ou não (algumas linguagens aceitam diferentes tipos de dados em um mesmo array, outras não), os arrays são usados para armazenar vários dados em uma mesma estrutura. 

Os "Arranjos" são enumerados (começando pelo 0) por índices, facilitando muito encontrar itens especificos, sendo necessário apenas usar seu endereço dentro do array, outro ponto importante é que os itens estão "encadeados aos outros", tornando a <b>leitura muito simples e rápida</b>, mas isso também implica em dificuldades em inserir e retirar dados, uma vez que arrays são alocados na memória continuamente, então para inserir um novo item na lista, precisaríamos empurrar todos os dados subsequentes para seus próximos indicies ( oque por si só não é um grande problema), mas também precisamos nos certificar que há memória sobrando, caso não haja o array inteiro precisa ser realocado em algum espaço da memória que tenha espaço suficiente para todos os itens em fileira.</p>

---
---
<h4 id="Listas Encadeadas"> Listas Encadeadas .. </h4>

<p> As "Linked Lists" podem ser consideradas o completo oposto dos arrays, enquanto os arrays são de fácil leitura e processamento, e ineficientes na hora de inserir ou retirar dados, as listas tem como principal característica sua <b>Flexibilidade</b> na hora de inserir e excluir seu conteúdo, mas são ineficientes para processamento e leitura, exigindo mais tempo e performance do Hardware.

Isso acontece porque as listas encadeadas tem seus "nodes" ou nós, alocados na memória de forma independente, sem precisar de um grande espaço contínuo, e a lista mantém sua ordem através de <b>ponteiros</b> que ligam um dado no outro. Portanto, não é preciso realocar grandes quantidades de dados por vez, para inserir algo no meio da lista basta apenas alterar o ponteiro do elemento anterior e adicionar outro ligando o item atual ao seu sucessor, e por essa dinâmica de ponteiros e pela distância entre seus elementos, a lista exige mais processamento para ser lida, uma vez que para chegar ao seu último elemento, o computador precisa passar por todos os outros para obter seu endereço. </p>

---
---
