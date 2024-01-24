## BEM - bloco elemento modificador
Podemos perder o padrão do CSS e causar o efeito cascata. Para evitar isso, podemos adicionar mais especificidades aos seletores.
*cuidado* para não poluir os códigos
*nao esquecer de deixar a classe igual no html*
 Utiliza-se o __ para o elemento
 .topo__link {
    color:red;
 }
o modificador se usa --
.rodape__link--pequeno{
    font-size:12px
}

## SMACSS - scalable and modular architecture for css
Arquitetura escalavel e modular para o css 
- BASE- tudo que estiliza os elementos, pseudos seletores e estilos globais. Ex: div,section.. Não deve conter id e etc

- Layout - elementos que são unicos na nossa página e, geralemente, representam as partes grande do nosso site. Ex: head, mais, footer...

- Module - Elementos que são reutilizados em diversos locais. Ex: botões, listas ..

- State - modificadores dos nosso elementos. Ex: quando um botão está em foco quando um elemento deve desaparecer....

- Theme - Geralmente ficam cores dos temas, fontes e etc.

*sempre seguir um style guide*


## Frameworks
- Ferramentas que disponibilizam funcionalidade pré-prontas 

## CSS lint
- Analisa o código em busca de trechos fora do padrão 

## Normalize Css e ResetCSS