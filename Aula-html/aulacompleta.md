abirir o vscode 
criar o index.html 
clicar com botão direito no arquivo>open live server (minha porta http://127.0.0.1:5500/index.html)

se aperecer apenas o numero 
digitar local host+ numero que apareceu 
Digite o texto, sempre que salvar atualiza automaticamente a pagina da web

html é estruturado em tag e devem ser abertas e fechadas
ex: <p> exemplotag </p> - tudo isso forma elemento (p se refere a paragrafo)

### aninhamento de elementos
inserir um elemento dentro do outro. *a ultima tag a ser aberta deve ser a primeira a ser fechada*

### atributos - propriedades 
o atributo constitui valor a uma tag 
ex: class="exemplo">exemplo de atributo

Sempre inicia com tipo de documento, na parte head se coloca tudo que o usuário nao vai ver

title da pagina não é o h1 (titulo do body), podendo ser até 6 *mantém-se a hierarquia dos elementos*

importante identificar o atributo da lingua (lang= ptBr)

Pode-se enfatizar com <em> e deixar mais "forte" com <strong>

### lista
lista ordenada - <ol>
cada item da lista <li>

lista desordenada <ul>
lista aninhada uma ol com ul

### link 
para colocar um link se coloca <a href="endereço" </a>
se insere um title no link, como uma descrição

para abrir em nova aba se usa <target="_blank" rel=noreferrer noopener> para nao atribuir referencia e valores do site aberto com o seu site 

### formulários
para criar, se usa a tag <form>
*label etiqueta do campo e input é onde o usuário pode preencher*

type passaword esconde os caracteres

elemente <textarea> é igual o input mas permite ter mais de uma linha

o atributo for indica valor/referencia a um elemento

o atributo placeholder dá a sugestão para o usuário

## botão 
tag <button>, se *submit* ele envia a msg e limpa os campos

### tags

tag Img (imagem), geralmente conjunto com o tributo src que diz onde a imagem está, a imagem tambem permite title (para legendar ao passar o mouse)

figcaption quando precisamos da legenda na tag figure

### tabela
tag table para criar tabela
tag td para colunas 
tag tr para linhas
tag caption para dar nome a tabela

### tags comuns
<header> indica que o conteudo esta dentro do cabeçalho, geralmente tem logo, menu de navegação e deve ficar no body

<main> conteudo principal, nao pode estar dentro de uma tag article, assaid, footer, reader ou nave e só deve ter uma tag main

<footer> o rodapé do site, geralmente direitos autorais e autor

<nav> links de navegação 

<asaid> conteudo relacionado ao main

<article> geralmente utilizado em blog

<section> apresenta uma seção (precisa ter um alemento de cabeçalho )

<div> <span> tag generica, sem valor semântico mas agrupa elementos e estiliza a pagina






