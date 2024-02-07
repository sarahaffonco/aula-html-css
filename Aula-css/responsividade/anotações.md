Responsividade - conjunto de tecnicas para adptar uma página, independente de onde o usuário acessar. 

## Media Queries 
Cria-se codigos css que são utilizadas em momentos especificos 
Ex 
.caixa{
    width: 300px;
    height:300px;
    background-color: green;
    }
*midia querie*
@mmedia (max-width: 600px) {
    .caixa{
        background-color: pink;
    }
}

- Viewport
É a janela em que a página é exibida.
precisamos identificar a tela que está sendo exibida
dentro do head adicionamos:
<meta
    name="viewport"
    content="width=device-width, initial-scale=1.0"
    >

## Unidades de medidas flexiveis
- Max Width - controla a unidade de medida para imagem mantenha o tamanho normal mas se torna flexivel
ex: max-width: 256px;

## Imagens
Tendem a ser um arquivo grande e pod demorar para carregar, dependendo da internet. Podemos resolver a demora com o carregamento de uma imagem por vez e do tamanho da tela.
- srcset - o html seleciona qual carregar primeiro
ex: <img srcset = "imagens/gatopqno.jpg 200w,
                    imagens/gatognde.jpg 718w
                    sizes ="(max-width:200px)" 200px, 700px
    >

## Media Queries 
GAP: nPX
(assim o conteúdo vai se adaptando conforme o tamenho)

https://www.w3schools.com/css/css_rwd_mediaqueries.asp

https://developer.mozilla.org/pt-BR/docs/Web/CSS/CSS_media_queries/Using_media_queries

https://cursos.alura.com.br/course/html-css-responsividade-publicacao-projetos/task/121397

@media (max-width: 1200px ){
    .apresentacao{
        flex:direction:column-reverse;
    } 
}
