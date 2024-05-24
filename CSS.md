## Cascading Style Sheets

<b></b>

--- 

### Sumário:


<a href=#CSS>- CSS</a> <br>
<a href=#Flexbox>- Flexbox</a><br>



---

<pre>
 ________          ________           ________      
|\   ____\        |\   ____\         |\   ____\     
\ \  \___|        \ \  \___|_        \ \  \___|_    
 \ \  \            \ \_____  \        \ \_____  \   
  \ \  \____        \|____|\  \        \|____|\  \  
   \ \_______\        ____\_\  \         ____\_\  \ 
    \|_______|       |\_________\       |\_________\
                     \|_________|       \|_________|
                                                    
                                                    
</pre>

---

<br><br><br><br><br><br><br><br><br>

---

<p id="CSS">O CSS surgiu devido a necessidade de estilizar as páginas html de uma forma eficiente e produtiva. </p>

---
### Exemplo de sintaxe:

---

<pre>body {
    background-color: Black
    xxxxx
    xxxxx
} 
</pre>

Já falando de "box-model", o padding é a distância entre o conteúdo e sua borda, enquanto a margem é a distância entre a borda e os outros elementos. 

E SEMPRE o primeiro valor vai ser a altura e o segundo a horizontal.

Pensando em produtividade, é interessante usar as classes para facilitar o desenvolvimento. Tudo que é preciso fazer é adicionar o atributo <h1 "class="xxx"> e no arquivo css usar o "." para identificar as classes.

---

#### É muito importante nomear as classes de forma direta e sucinta para facilitar a leitura do código.
##### Pensando nisso, posso me basear no padrão *BEM*, no caso Block Element Modifier, que aconselha a criação de nomes seguindo essa ordem, primeiro o bloco de determinado elemento, depois o elemento e por último o modificador que o elemento pode ter, como ativo ou não. 
##### Por exemplo: *header-item-active*

### Boas práticas:

#### O "CSS Reset" literalmente reseta os padrões de estilo dos navegadores e confere mais controle ao dev e uma padronização mais confiável em diferentes navegadores. Um exemplo de CSS Reset: 
##### ( O asterisco serve para identificar todos os elementos do html ).

##### * {
    padding: 0
    margin: 0
}

##### É interessante já começar a estilização com alguns padrões como definir o body como height: 100vh; (O que define que o body vá cobrir a página inteira, sem scroll), e para evitar que as imagens saiam da página ( ou simplemente um elemento filho não saia do elemento pai), usamos o "box-sizing: Border-box;" no elemento pai.


---

<br>
<br>

<h2 id="Flexbox">Flexbox</h3>


<p> Para preservar a responsividade do site, não é interessante manipular diretamente o posicionamento dos elementos usando medidas como pixels, por isso é interessante usar a ferramenta "Flexbox".</p>

---

#### Display: Flex ;

- Para começar a usar as funções é necessário usar o "display: flex;" no elemento pai, para conseguir manipular os elementos filhos.</p>

#### Flex-direction: 

- O Flex direction define o eixo (ou direção) dos itens dentro da DIV, seu parâmetro default é <b>"Row"</b> que define o eixo como horizontal, e também podemos usar o <b>"column"</b> para o eixo vertical. 

        Também é possível usar o inverso dos dois acima, row-reverse e column-reverse.

#### Flex-wrap: 

- Define se os itens deverão se "espremerem" ou se podem usar outras linhas para preservar seu tamanho original. Seus parâmetros são:


         nowrap, wrap, wrap-reverse

#### Justify-content: 

- Essa função serve para alinhar seus itens com o eixo estabelecido. Seus possíveis parâmetros são:

       Justify-content: Flex-start (Padrão), flex-end, center, baseline, space-between, space-around, space-evenly

#### Align-items : (COM EME MMMMMMMMM não n)
- Serve para alinhar os itens com o eixo vertical (tecnicamente o transversal, mas vertical é mais lúdico)

        Align-items: stretch (padrão), flex-start, flex-end, center, baseline

#### Align-content :
- Usado para múltiplas linhas de conteúdos, alinha o espaço entre os itens.

        align-content: stretch (padrão), flex-start, flex-end, center, space-between, space-around

#### Align-self :
- Usado para alinhar um item individualmente, mesmo dentro de um conteiner com outro "align".

        align-self: flex-start, flex-end, center, baseline, stretch

---



<br>
<br>


























### Links Úteis:

https://fonts.google.com/


https://css-tricks.com/snippets/css/a-guide-to-flexbox/

https://www.interaction-design.org/literature/topics/ux-design

https://css-tricks.com/

https://www.alura.com.br/artigos/css-seletores-avancados-aplicacoes-web?_gl=1*q2pajr*_ga*MTUyNzA3NjcxMy4xNzA1NjIyNTg1*_ga_1EPWSW3PCS*MTcxNTM4MjE3NC4zNS4xLjE3MTUzODY3NTYuMC4wLjA.*_fplc*V3lPdVFkSEZXdEtwdSUyRmZpR0pxYXdEbGFmSHNXOGV0bFlQalhQbyUyRlBEWGhBJTJGOXJwcU9HM3RpJTJCWGNlNld1NWxhNE9ONDlVNmk3NXYlMkJqMEpxVmYyWk5PUjBZUUVLclM2ciUyRk9NYVFESFBIZVNnclRYaDU2JTJGJTJGcWdCTUUybm04QSUzRCUzRA..

https://www.alura.com.br/artigos/comecando-a-organizar-seu-css?_gl=1*1slkysh*_ga*MTUyNzA3NjcxMy4xNzA1NjIyNTg1*_ga_1EPWSW3PCS*MTcxNTM4MjE3NC4zNS4xLjE3MTUzODY4MTkuMC4wLjA.*_fplc*V3lPdVFkSEZXdEtwdSUyRmZpR0pxYXdEbGFmSHNXOGV0bFlQalhQbyUyRlBEWGhBJTJGOXJwcU9HM3RpJTJCWGNlNld1NWxhNE9ONDlVNmk3NXYlMkJqMEpxVmYyWk5PUjBZUUVLclM2ciUyRk9NYVFESFBIZVNnclRYaDU2JTJGJTJGcWdCTUUybm04QSUzRCUzRA..

Coolors

Adobe color wheel






