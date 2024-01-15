##CSS
*cascading style sheets*
Folha de estilo em cascata

Existem 3 formas de utilizar o CSS

In Line - <style="informação do atributo>

Interna - dentro da head <style> p {color} </style>

Externa - abrindo um novo documento no .css;
"adiciona o css com a tag <link> que fica no head. ex <link rel="stylesheet" href="estilo.css">
Css é composto pelas regras
p (seletor) {propriedade:valor} (todo {} é uma declaração)

*seletores css*
Seletor Tipo/elemento - seletor do elemento p (irá alterar o estilo de todos elementos p)

Seletor Classe - como se fosse um apelido do elemento ".classe" 

Seletor de iD - No html se coloca id="nomedoid"; e no css #nomedoid

Seletor global - representado por *, seleciona todos os elementos da página

Seletor de descendente - selecina todos elementos aninhados, em todos os niveis. Se não quiser que todo o elemento da main mude o estilo, se usa o seletor de "filho" main >h3 (somente os h3 que estiverem devidamente aninhado com a main, será selecionado).

*Pseudo Seletores/pseudo classes*
Pseudo elemento, criamos elementos para estilizar
Seletor Hover - faz com que a regra Css aplica o estilo apenas quando passamos o mouse em cima do elemento.

Seletor Focus - aplica a regra quando o elemento estiver focado (tab)

Seletor Active - aplica a regra quando usuário clicar no elemento ou enquanto o elemento estiver pressionado.

Seletor first Child -  seleciona o primeiro elemento filho encontrado na pagina.

Seletor last-child - seleciona o ultimo elemento.

Nth-Chil - seleciona o que optamos.
ex: li:nth-child (2) (item 2) 
nth-child (odd) (impar)


*Pseudo-elementos*
Permite estilizar uma parte especifica do elemento selecionado, ou criar uma parte do elemento selecionado

After - cria elemento como ultimo filho do que selecionamos

Before - Cria elemento como primeiro filho do elemento selecionado

~nos pseudo elementos utilizamos ::, diferente da pseudo classe.

*Declarando cor*

Escrever o nome da cor em ingles {color:green}

RGB (red green blue) - representa as cores em escala, enumeradas de  a 255 para indicar a quantidade de cor.

Hexadecimal - reduz as cores em caracteres.

*Unidade de medida*

Pixel - define um tamanho estático para elemento ou propriedade CSS.

