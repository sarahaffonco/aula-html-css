# CSS
*cascading style sheets*
Folha de estilo em cascata.

Existem 3 formas de utilizar o CSS:

- In Line - <style="informação do atributo>

- Interna - dentro da head 
Ex: <style> p {color} </style>

- Externa - abrindo um novo documento no formato .css;
"adiciona o css com a tag <link> que fica no head. 
Ex <link rel="stylesheet" href="estilo.css">

Css é composto pelas regras:
p (seletor) {propriedade:valor} (todo {} é uma declaração)

## seletores css
- Seletor Tipo/elemento - seletor do elemento p (irá alterar o estilo de todos elementos p)
Ex: p {
    color:green;
}

- Seletor Classe - como se fosse um apelido do elemento ".classe" 
Ex:.roxo {
    color:purple
}


- Seletor de iD - No html se coloca id="nomedoid"; e no css #nomedoid.
Ex:#paragrafo {
    color:brown
}

- Seletor global - representado por *, seleciona todos os elementos da página.
Ex: *{
   color: pink;
}

- Seletor de descendente - selecina todos elementos aninhados, em todos os niveis. Se não quiser que todo o elemento da main mude o estilo, se usa o seletor de "filho" main >h3 (somente os h3 que estiverem devidamente aninhado com a main, será selecionado).
Ex: main h3 {
    color:red
}


## Pseudo Seletores/pseudo classes
Pseudo elemento, criamos elementos para estilizar, sendo eles: 

- Seletor Hover - faz com que a regra Css aplica o estilo apenas quando passamos o mouse em cima do elemento.
Ex: .exemplo:hover {
    background-color: pink;
}

- Seletor Focus - aplica a regra quando o elemento estiver focado (tab).
Ex: .exemplo:focus {
    background-color: pink;
}

- Seletor Active - aplica a regra quando usuário clicar no elemento ou enquanto o elemento estiver pressionado.
Ex: .exemplo:active {
    background-color: lightslategrey;
}

- Seletor first Child -  seleciona o primeiro elemento filho encontrado na pagina.
Ex: li:first-child {
    color:blue
}

- Seletor last-child - seleciona o ultimo elemento.
Ex: li:last-child {
    color:red
}

- Nth Chil - seleciona o que optamos.
ex: li:nth-child (2) (item 2) 
nth-child (odd) (impar).
Ex: li:nth-child(2) {
    color: green;
}


## Pseudo-elementos
Permite estilizar uma parte especifica do elemento selecionado, ou criar uma parte do elemento selecionado.

- After - cria elemento como ultimo filho do que selecionamos
Ex:.exemplo::after {
    CONTENT: "DEPOIS";
}

-Before - Cria elemento como primeiro filho do elemento selecionado.
Ex: .exemplo::before {
    CONTENT: "ANTES";
}

*nos pseudo elementos utilizamos ::, diferente da pseudo classe*

## Declarando cor

- Escrever o nome da cor em ingles {color:green}.
Ex: .exemplo {
    Color: green
}

- RGB (red green blue) - representa as cores em escala, enumeradas de  a 255 para indicar a quantidade de cor.
Ex: .exemplo {
    color: rgb (255,50,0)
} 

- Hexadecimal - reduz as cores em caracteres.
Ex: . exemplo { color: #ff0000 }


## Unidade de medida

- Pixel - define um tamanho estático para elemento ou propriedade CSS.
ex: .exemplo {
    height: 150px; /*largura*/;
    width: 150px; /*altura*/
} 

- Porcentagem - tamanho relativo.
Ex: .exemplo {
    height: 100%; /*largura*/
   }

## Fontes
Pode-se alterar o nome da fonte e o estido da fonte de todos textos.
Caso necessário inserir mais de duas fontes, as fontes ficam entre virgulas. Ex: verdana, Aria, Sans-serif.
Ex:  .texto {
    font-family: cursive;
   }

Também podemos importar a fonte no html:
google Fontes - Select this style > copia o código que o próprio google livera e colocar na head e assim coloca a fonte no css.

**Opções mais comuns de Display**
o valor de display já é pré definido nos navergadores.

- Display Block - se comporta como um bloco na página, ocupando a linha inteira mesmo que não for definido um valor.
Ex: .texto {
     background-color: green display:inline; 
     }

- Display Inline - ocupa somente o texto, como uma caixa. Não aceitam propriedade de altura e largura, para isso se usa o inline-block.
Ex: .texto {
    background-color: green
    display:inline;
   }

Display inline-block - permite que os elementos se comportem corretamente ao receber algumas propriedades.
Ex:  .link {
    background-color: green
    padding:15 px;
    display: inline-block;
   }

Display None - faz com que o elemento não seja exibido na tela.
Ex:   .link {
    background-color: green
    padding:15 px;
    display: none;
   }

## Posicionamento 

- Position static - valor padrão de posicionamento e nao pode ser alterado


- Position Relative - é uma posição relativa, e pode ser alterada.
Ex:  .caixa {
    background-color: green;
    width: 150px;
    height: 150px;
    position:relative;
    top: 100px;
    left: 50px
    z-index:2;
   }

- Position absolut - irá se posicionar na tela ignorando todos elementos, pode ocorrer uma sobreposição de elementos.
Ex: .caixa-absoluta{
    background-color: blue;
    width: 100px;
    height: 100px;
    position:absolute;
    top: 50px;
    left: 45px
   }

   
   .caixa-absoluta{
    background-color: blue;
    width: 100px;
    height: 100px;
    position:fixed;
    top: 10px;
    
   }

*propriedade z-index, especifica a ordem de profundidade. A propriedade maior fica por cima da propriedade menos

Position fixed - fica fixo na pagina.

## Espaçamento

- Propriedade Margem - podemos declarar de 4 formas 
Valor.
Ex: width: 100px;
    height: 100px;
    Margin: 100px

- Valor especifico 
Ex:  width: 70px;
    height: 70px;
    margin-top: 20px;
    margin-right: 5px;
    margin-bottom: 10px;
    margin-left: 15px;

- Margem abreviada
Ex: margin: 5px 10px 15px 20px
 top;right;left;right;

- Margens iguais
Ex: margin: 30px 40px

# padding 
Define o espaçamento interno dos elementos (distancia do elemento para a borda dele); pode-se declarar igual a margem.
o valor do padding é somado ao valor total do elemento; para evitar essa soma utilizamos a propriedade box-sizing
Box-sizing Border-box - o elemento terá os valores que definimos, o padding passa a ser conjunto ao valor total ao invés de somada
Ex: .botao {
    padding: 5px 20px;
    width: 50px;
    height: 50px;
    Box-sizing: Border-box;
   }

## Estilos padrões dos elementos
- Cada navegador adiciona o seu próprio estilo CSS, para verificar os padrões basta "inspecionar " na página da web.

## Propriedades genéricas - Textos

### Borda
Temos duas maneiras de declarar a borda: de forma resumida e de forma especifica.
Para arredondar os cantos da borda, se usa border-radius.
Ex: 
   .caixa-1{
    border: 1px solid red;
    border-radius:10px;
    box-shadow:5px 5px 10px 5px black
    }

   .caixa-2{
    border-width:1px
    border-style:solid
    border-color:green
   }

Box-shadows - adiciona efeito sombra aos elementos.
Ex:  box-shadow:5px 5px 10px 5px black 
box-shadow: eixo horizontal; eixo vertical; desfoque;propagação e cor. 


Cursor - altera o estilo do cursor.
Ex: 
   .botão{
    cursor:pointer
   } 

Overflow - Ignora o conteudo que não "cabe" nas dimenções da caixa
Overflow:scroll - cria uma barra de rolagem dentro da caixa.

### Estilizar textos
Fonte size - Controla o tamanho da font
Ex: font-size: 12px

- Font-wight - altera o peso (como se fosse negrito)
Ex: font-wight:bold

- Text align - para alinhar o texto, aceita os valores: center, justify, left, right...

Text indent - define o espaço antes de iniciar uma linha de texto
ex: texte-indent:20px

Latter Space - determina o espaçamento do conteúdo.
Ex: latter-spacing: 5px

Line Height define a altura da linha do texto
Ex: line-height: 40px

## Principais propriedades - Listas
- List style - controla os principais marcadores da lista.
Ex: .lista {
    list-style:none
}
*none - não exibe nenhum marcador;*
*Square - os marcadores são quadrados;*
*lower-roman - exibe os marcadores em romanos.*

## Principais propriedades - Link
Existe um padrão.
Atenção para nao esquecer nenhum comando importante.
Quando passamos o valor # no link, quer dizer que não leva a nenhuma página *não pode acontecer*
*html* <a href=# class="link"> Clique aqui.</a>

- Text decoration - remove o sublinhado do link
Ex: .link {
    text-decoration:none;
    color: tomato;
    }   

- Hover - ao passar o mouse por cima do link, altera a cor.
    . link:hover{
        color:violet;
        
    }

- Active - quando o link for clicado ou pressionado.
    .link: active {
        color:darksalmon
    }

- Focus - quando o elemento está focado.
    .link:focus {
        outline: none;
        border: 1px solid tomato
    }

## Principai propriedades -outras
- Background Image - permite colocar um background no elemento sem inserir a imagem no html.
*html <div class="caixa"></div>
Ex: . caixa {
    width: 400px;
    height: 400px;
    border: 1pc solid green;
    Background-image:url('imagem.jpg");
}
*pode acontecer um erro de tamanho, para resolver a repetição, basta usar "background-repeat:no-repeat;"*

*controlar a posição da imagem "background -position: 10px 40px" ou "background -position: center"

*alterar o tamanho da imagem "background-size: 50px 60 px"


## Principais conceitos CSS

- Efeito cascata - a última regra que fica vigente. 

- Herança - O Css se comporta passando estilo de pai para filho. 
ALguns valores não passam por herança como as propriedades de box model (width, heigh, paddington); para forçar a herança se usa inherit.
Ex: .elemento-filho {
    width: inherit;
}

- Calculo de espcificidade - seletores diferentes, tem pesos diferentes independente da cascata.
O seletor mais especifico tem vantagem (precedência) pelo seletor mais generico.
Existe um valor para cada tipo de elemento e asssim vemos sua especificidade.
*calculo* /*10 +10 +10 =30 * (cada tipo de seletor tem um valor.. seletor de classe = 10 pontos, seletor de elemento 1 ponto, seletor de id 100 pontos)

## Animações com CSS
Podemos controlar as mudanças de cor para suavizar, isso ocorre pela propriedade transition.
Ex: .botao {
    background-color: #e768f2;
    transition: background-color .5s;

}

Devemos imaginar as animações sempre como uma linha do tempo, com começo meio e fim.
regra "@keyframes".
Ex: @keyframes animacao {
    0% { 
        background-color: pink
    }
    100% {
        Background-color:purple
    }
    
}
.caixa {
    width: 300px;
    height: 300px;
    animation: animacao 1s infinite;
}

### Performace em animações
*cuidado para não travar o computador do usuário*
Para animar alguma propriedade, pode-se usar o will-change para melhorar o desempenho
Ex: will-change: left e top

## Trabalhando com  Transformações
### Scale
o valor scale é utilizado para transformar a escala do elemento. O valor scale pode variar conforme o eixo (x/y) scaleX(.3).
Essa transformação só é feita no próprio intem.
Ex: .caixa {
    width: 300px;
    height: 300px;
    Background-color:purple;
    transform: scale (2)
}

### Rotate
O rotate faz com que o elemento rotacione
ex:width: 300px;
    height: 300px;
    Background-color:purple;
    transform:rotate (35deg)

També podemos utilizar pelo @keyframes
width: 300px;
    height: 300px;
    Background-color:purple;
    animation: girando 2s infinite;

@keyframes girando {
    transform: rotate (0deg);
}

    100% {
        transform: rotate (360deg);
    }

### Translate 
Transforma a posição dos elementos. 
Também podemos alterar somente na ordenada x ou y.
Ex: width: 300px;
    height: 300px;
    Background-color:purple;
    transform:translate (30px, 30px)

### Skew
Utilizado para distorcer o elemento.
Também podemos alterar somente na ordenada x ou y.  
 Ex: width: 300px;
    height: 300px;
    Background-color:purple;
    transform:skew (10deg)

### Opacity
Altera a opacidade de um elemento, por não ser necessária a transformação, usa-se somente o comando.
 Ex:.botao {
    opacity: .5
 }

 ## Css Layouts - Box Model
 Para analisar ou construir um layout, precisamo entender sua função individual.
 o Box Model descreve as caracteristicas que definem o espaço de um elemento na página. 
 Cada elemento tem 4 áreas especificas (edges)
  - Area de conteudo - content ed; é o espaço dentro do elemento onde podemos adicionar qualquer conteudo, pode ser alterada com as propriedades de altura e largura. 
  As edges podem ser vizualidas na area elements do navegador.
  Margin Edge
  Border Edge
  Padding edge
  Ex: width: 100px;
    height: 100px;

## Css Layouts - Flex-box
Geralmente lida com o elemento pai (flex container). 
*html* cria uma div class=container
Ex: .container {
    border: 1px solid green;
    display: flex;
}

### Propriedades do Flex-box
- Flex direction - controla a direção dos flex, seu padrão é row e se comportam como linha.
Ex: border: 1px solid green;
    display: flex;
    flex-direction: row-reverse;

- Flex-Wrap - altera o comportamento quando redimensionamos a janela, o comportamento padrão (nowwrap) é se ajusta diminuindo seu tamanho, ao utilizar o wrap elas se comportam criando uma nova linha.
Ex: border: 1px solid green;
    display: flex;
    flex-wrap: wrap

- Flex-flow - tambem podemos chamar de  shorthand para flex direction e flex wrap. Podemos utilizar doi valores wrap e direction.
Ex: border: 1px solid green;
    display: flex;
    flex-flow: row-reverse wrap

- Justify-content - permite alinhar os itens horizontalmente. 
o valor padrão é Flex Start (alinha no começo da linha, a esquerda).
Essa propriedade não funciona se utilizarmos flex-wrap: wrap;
Valores: end, center, space-between (espaços iguais); space-around;space-evenly.
Ex: border: 1px solid green;
    display: flex;
    justify-content: flex-end

- Align-items - alinha os elementos verticalmente, valor padrão é stretch.
Valores: flex -start (cada item tem altura de acordo com o conteudo) ; flex-end (alinha na parte inferior); flex-center
Ex: border: 1px solid green;
    display: flex;
    height: 300pc
    align-items: flex-end

- Align-Content  - alinha os flex itens em flex container e permite mais de uma linha.
Valores: stretch (forma linhas); start (tem a altura definido pelo conteudo) center, end, epace-between, space around
Ex: border: 1px solid green;
    display: flex;
    height: 300pc
    flex-wrap: wrap
    Align-content: stretch

- Order - modifica os flex itens e não o flex container. Para definir order, temos que redefinir os valores de todos intens
Valores: 
Ex: .caixa: nth-child (3)
    order: 1

- Grow - modifica o tamanho do item, se necessário. Por padrão odo grow é 0.
Quanto maior o valor, maior a caixa do item.
Ex: .caixa: nth-child (3).
    flex-grow: 1

Não finalizado modulo 11








