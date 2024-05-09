## Cascading Style Sheets

O CSS surgiu devido a necessidade de estilizar as páginas html de uma forma eficiente e produtiva. 

### Exemplo:

body {
    background-color: Black
    xxxxx
    xxxxx
} 

Pensando em produtividade, é interessante usar as classes para facilitar o desenvolvimento. Tudo que é preciso fazer é adicionar o atributo <h1 "class="xxx"> e no arquivo css usar o "." para identificar as classes.

#### É muito importante nomear as classes de forma direta e sucinta para facilitar a leitura do código.
##### Pensando nisso, posso me basear no padrão *BEM*, no caso Block Element Modifier, que aconselha a criação de nomes seguindo essa ordem, primeiro o bloco de determinado elemento, depois o elemento e por último o modificador que o elemento pode ter, como ativo ou não. 
##### Por exemplo: *header-item-active*

#### Outra coisa importante é o "CSS Reset", que literalmente reseta os padrões de estilo dos navegadores e confere mais controle ao dev e uma padronização mais confiável em diferentes navegadores. Um exemplo de CSS Reset: 
##### ( O asterisco serve para identificar todos os elementos do html ).

##### * {
    padding: 0
    margin: 0
}