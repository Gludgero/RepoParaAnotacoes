## Cascading Style Sheets

O CSS surgiu devido a necessidade de estilizar as páginas html de uma forma eficiente e produtiva. 

### Exemplo:

##### body {
    background-color: Black
    xxxxx
    xxxxx
} 

Pensando em produtividade, é interessante usar as classes para facilitar o desenvolvimento. Tudo que é preciso fazer é adicionar o atributo <h1 "class="xxx"> e no arquivo css usar o "." para identificar as classes.

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

### Flexbox

Documentação usada para pesquisas: 
https://css-tricks.com/snippets/css/a-guide-to-flexbox/

##### Para preservar a responsividade do site, não é interessante manipular diretamente o posicionamento dos elementos usando medidas como pixels, por isso usar a ferramenta Flexbox.

##### Pra começar é necessário usar o "display: flex;" no elemento pai, para conseguir usar o fbx nos elementos filhos.

##### Para alinhar os elementos com os outros elementos (não alinhar os elementos com a página), usa-se o align-itens: xxxx












