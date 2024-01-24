# Aprendendo Html
abirir o vscode
criar o index.html 
clicar com botão direito no arquivo>open live server (minha porta http://127.0.0.1:5500/index.html)

se aperecer apenas o numero:
digitar local host+ numero que apareceu;
Digite o texto, sempre que salvar atualiza automaticamente a pagina da web.

html é estruturado em tag e devem ser abertas e fechadas.
ex: <p> exemplotag </p> - tudo isso forma elemento (p se refere a paragrafo).

*Padrão Html*
Ex: <!DOCTYPE html>
<html lang="pt-BR">
    <head>
        <meta charset="utf-8>"
        <title> WomakerdCode</title>
        <meta name=""author" content="Sarah Affonco">
        <meta name="description" content="Aula sobre HTML5 e CSS3 -WoMakersCode"

    </head>

    <body>
        </body>
</html>

## Aninhamento de elementos.
inserir um elemento dentro do outro. *a ultima tag a ser aberta deve ser a primeira a ser fechada*.

## Atributos - propriedades 
o atributo constitui valor a uma tag.
ex: class="exemplo">exemplo de atributo.

Sempre inicia com tipo de documento, na parte head se coloca tudo que o usuário nao vai ver.

title da pagina não é o h1 (titulo do body), podendo ser até 6 *mantém-se a hierarquia dos elementos*.

Importante identificar o atributo da lingua (lang= ptBr).
Ex:     <p lang=""en">this is a paragraph in english</p>

Pode-se enfatizar com <em> e deixar mais "forte" com <str<p> Enfase <em> aqui </em> e <strong> importância</strong></p>ong>.
Ex: 

## Lista
lista ordenada - <ol>.
cada item da lista <li>.
Ex:  <ol>
            <li> item 1 </li>
            <li> item 2</li>
        </ol>

lista desordenada <ul>.
lista aninhada uma ol com ul.
Ex: <ul>
            <li> item 1
            <li> item 2</li>
            </li>
        </ul>

## Link 
Para colocar um link se coloca <a href="endereço"> </a>.
se insere um title no link, como uma descrição.
Ex: <p> este é um link para o <a href="https://github.com/sarahaffonco" tittle="github da desenvolvedora"
     target="_blank" rel="noreferrer noopener"> github</a>.</p>

Para abrir em nova aba se usa <target="_blank" rel=noreferrer noopener> para nao atribuir referencia e valores do site aberto com o seu site.

## formulários
Para criar, se usa a tag <form>.
*label etiqueta do campo e input é onde o usuário pode preencher*.

Type passaword esconde os caracteres.

elemente <textarea> é igual o input mas permite ter mais de uma linha.

Ex:<form>
            <div>
                <label for="nome">Nome:</label>
                <input type="text" id="nome" placeholder ="digite seu nome">
            </div>

             <div>
                <label for="mensagem">Mensagem:</label>
                <textarea id="mensagem">Mensagem pronta</textarea> 
            </div>


o atributo for indica valor/referencia a um elemento

o atributo placeholder dá a sugestão para o usuário

## Botão 
tag <button>, se *submit* ele envia a msg e limpa os campos
Ex: <div>
                <button type="submit"> Enviar Mensagem</button>
            </div>
            

## Tags
Tag Img (imagem), geralmente conjunto com o tributo src que diz onde a imagem está, a imagem tambem permite title (para legendar ao passar o mouse)

figcaption quando precisamos da legenda na tag figure

Ex: <img src="imagem/people.png" alt="criança negra com a mao na boca">
            
            <figure>
                <figurecaption> Bebe negro com a mão na boca e pijama azul</figurecaption>
            </figure>


## Tabela
tag table para criar tabela
tag td para colunas 
tag tr para linhas
tag caption para dar nome a tabela

Ex: <table>
                    <caption>Datas de Aniversário</caption>

                    <tr>
                        <td>Nome</td>
                        <td>Idade</td>
                        <td>Aniversário</td>
                    </tr>

                <tr>
                    <td>Sarah</td>
                    <td>28</td>
                    <td>12/94</td>
                </tr>
                </table>

## Tags comuns
<header> indica que o conteudo esta dentro do cabeçalho, geralmente tem logo, menu de navegação e deve ficar no body.
Ex:  <header> Cabeçalho </header>

<main> conteudo principal, nao pode estar dentro de uma tag article, assaid, footer, reader ou nave e só deve ter uma tag main.
Ex:<main> conteudo principal</main>

<footer> o rodapé do site, geralmente direitos autorais e autor.
Ex: <footer>rodapé</footer>

<nav> links de navegação
Ex:  <nav> 
        <ul>
            <li><a href=#>página inicial</a></li>
            <li><a href=#>sobre</a></li>
            <li><a href=#>contato</a></li>
        </ul>
    </nav> 

<aside> conteudo relacionado ao main.
Ex: <aside> COnteudo referente ao main</aside>

<article> geralmente utilizado em blog.
Ex:  <article>
            <h3> Um artigo do site</h3>
            <p> esse artigo é um teste</p>
        </article>

<section> apresenta uma seção (precisa ter um alemento de cabeçalho).
Ex:<section> essa seção é boa</section>

<div> <span> tag generica, sem valor semântico mas agrupa elementos e estiliza a página.
Ex:  <span> 
            <p>utilizando em textos</p>
        </span>

## Gerenciamento de foco - acessibilidade
Caso queira, a parte visivel do foco deve ser estilizada e nao retirada
<tabindex> informa a ordem de foco (navegação por teclado) dos elementos da página
<tabindex="1">primeiro elemento a ser focado

<tabindex="0"> todos elementos, automaticamente

### semântica
usar o código como foi criado, um código limpo facilita uso em app móvel, deixa o site entre melhores resultados no mec. de busca.

o que devemos fazer? manter a estrutura, layout consistente, de maneira clara e objetiva 

html - estrutura
css - estilização

## wai-aria -accessible rich internet applications
São especificação do w3c para melhorar a acessibilidade.
Regras:
- Preferencia para utilizar os elementos semânticos;
- Não alterar a semantica padrão do elemento;
- Não se oculta elementos interativos e devem ter a semantica correta;
- Textos interativos devem ser descritivos;
- Todos elementos interativos devem poder ser utilizados atravéd do teclado;
- Não esquecer que usuario pode acessar o site de qualquer dispositivos.

### ARIA roles - funções:
Utilizamos para indicar o que elemento faz, não seja redundante!
ex: <form role="search"></form>
<nac role="navigation"></nav> - redundante
*existe um site com todos aria roles*

### Aria properties - propriedades:
utilizado para adicionar semântica nos elementos que não a tem por padrão
Utilizamos atributos com prefixo "aria".
ex: <button aria-haspopup="true"></button>

### Aria States - estados:
Utilizado quando desejamos informar a condição atual dos elementos 
Utilizamos aria-.
ex: <input type-"checkbox aria-selected="true">

Para testar, se usa leitores de tela.
Pode-se instalar pllugins para medir o nivel de acessibilidade ou sites que verificam.






