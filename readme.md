**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

# Programação Web - Laboratório 2: Explorando o HTML com o meu primeiro website  

**OBJECTIVO**: Nesta ficha criará um primeiro website que ficará disponível na nuvem onde irá aplicar os conceitos aprendidos na aula sobre HTML desta semana.

**PRÉ-REQUISITOS**: 
* Instale o VS Code para editar o código HTML de forma fácil. Senão, pode sempre usar o Notepad++. 
* Deverá ter feito o [lab1](https://github.com/ULHT-PW-2020-21/pw-lab1).
* Leia o enunciado todo antes de o começar a resolver para entender o que fará.

# 1. Estruturação

1. Crie uma pasta `projeto` 
1. Crie a pasta `lab1` que deverá conter o seu `lab1` criado na semana passada.
1. crie um ficheiro `lab1.html` que:
    * tenha como título "lab1" (usando a etiqueta `<title>` no `<<head>`)
    * tenha um cabeçalho `<h1>` a dizer "Lab1: Conhecer a Internet com a minha primeira página Web" 
    * tenha, numa lista, links para as duas páginas desse laboratório: `progweb.html` e  `report.html`.

1. Crie a pasta `lab2`
1. crie um ficheiro `lab2.html` que:
    * tenha como título "lab2" (etiqueta `<title>`)
    * tenha um cabeçalho `<h1>` a dizer "Lab2: Explorando o HTML com o meu primeiro website" 
    * deverá ter, numa lista, links para cada uma das páginas que irá criar neste laboratório.

1. crie dentro da pasta `projeto`o ficheiro `index.html` que:
    * tenha como título "Laboratórios Programação Web" (etiqueta `<title>`)
    * tenha um cabeçalho `<h1>` a dizer "Laboratórios Programação Web" 
    * deverá ter, numa lista, links para os ficheiros `lab1.html` e `lab2.html` (que estão nos seus respectivas pastas, pelo que deverá incluir no caminho o nome da pasta), usando o título de cada laboratório.

1. Os ficheiros `lab1.html` e `lab2.html` deverão ter um link para voltar para a landingpage do seu projeto, o ficheiro `index.html` na pasta `projeto`.

A estrutura final deverá ser como em baixo (com mais imagens na pasta img):
```
projeto
+-- index.html
+-- lab1
|   +-- lab1.html
|   +-- index.html
|   +-- report.html
|   +-- img
    |   +-- wordcloud.png
+-- lab2
|   +-- lab2.html
|   +-- ... (ficheiros a criar ao longo deste laboratório)
```

# 2. Cidade 

Fará neste laboratório 2 um website sobre uma cidade do mundo à sua escolha, que congregará várias informações que recolherá sobre esta. 

Um website é uma coleção de páginas HTML. Para tal, vamos criar um primeiro ficheiro, index.html, inserindo as partes elementares:

```html
<!DOCTYPE html>
<html lang="pt">
    <head>
    </head>
    <body>
    </body>
</html>
```

1. Na secção <head> especifique um título (etiqueta <title>) para a barra do navegador. 
2. Especifique também os seguintes metadados:
    1. codificação UTF-8. 
    2. nome do autor do site, email, data de criação, uma curta descrição do conteudo do site, e palavras chave.

<meta name="author" content="Ana Maria"> 
<meta name="keywords" content="palavras chave"> 
<meta name="description" content="Website sobre Lisboa">
<meta name="creation_date" content="date"
<meta name="contactNetworkAddress" content="seu@mail.com">

3. Crie um icon para o seu website. Para tal:
    1. Escolha uma imagem que converterá para icon (extensão .ico) recorrendo a uma aplicação web (e.g., https://www.favicon-generator.org/). Alternativamente, pode escolher um icon aqui https://www.iconspedia.com/.
    2. Guarde-o numa nova pasta `imagens`, dentro de `lab2`, 
    3. Insira um link para o icon no head da seguinte forma 
< link rel="shortcut icon" type="image/x-icon" href="imagens/favicon.ico"/>
    4. Poderá observar que, pelo facto de o icon estar na pasta “imagens”, tem sempre que especificar no href o caminho relativo para o local onde se encontra a imagem, o nome da pasta imagens (href="imagens/imagem.ico”).

4. Explore o site https://www.rapidtables.com/web/color/ , onde para cada cor existe uma palete de intensidades que pode escolher. Neste site, escolha uma cor clara para o fundo da sua página, e especifique-a através da etiqueta:
<body style="background-color:plum"> 

# 3. Criação do cabeçalho

Crie agora o cabeçalho do seu website. Terá o nome da Cidade, uma imagem e o menu, ficando da seguinte forma:

![](cabecalho.png)

Para, tal, siga os seguintes passos: 
1.	Na primeira linha insira o nome da cidade com o marcador `<h1>`.
2.	Na linha seguinte insira uma imagem da cidade a seu gosto. Redimensione a imagem para que tenha 300px de largura.No Paint existe uma opção resize que lhe permite escolher o número de pixels que pretende que tenha de largura. Respeite a proporção da imagem, sem a deformar! Guarde a imagem numa nova pasta `imagens`. Insira a imagem usando a etiqueta `img`. Deverá inserir depois desta uma quebra de linha, pois uma imagem não é um bloco.
3. Irá agora especificar o seu menu. Para tal
    1. Escreva o nome das páginas do seu site (Home, Localização, Multimédia, Informações) separados do carater `|`. 
    2. Para cada nome, crie um elemento hyperlink para a respetiva página (que criaremos a seguir):
        1. `index.html` para Home 
        2. `local.html` para Localização
        3. `multimedia.html` para Multimédia
        4. `info.html` para Informações


# 4. Criação das páginas do website

De seguida iremos criar as páginas do seu website que estarão interligadas.
1.	Crie 4 copias do ficheiro index.html que criou. 
2.	Altere os nomes dos ficheiros para ter um de cada, com os seguintes nomes: index.html, local.html, multimedia.html, info.html (atenção que os nomes dos ficheiros HTML  deverão estar em minúsculas, sem espaços, acentos ou carateres especiais)
3.	Em cada ficheiro, no menu ponha a negrito a palavra a que corresponde a página.
4.	Abra o ficheiro index, e experimente se os hiperlinks funcionam. 
Tem agora criado o seu website! Agora irá preencher cada página com conteúdos.

# 5. Página Home

1. Insira um parágrafo sobre esta cidade.
2. Pesquise na Internet por [carateres especiais UTF-8](https://www.w3schools.com/charsets/ref_html_utf8.asp) assim como por emojis na [W3Schools](https://www.w3schools.com/charsets/ref_emoji.asp) e na [emojipedia](https://emojipedia.org/): 
    1. Conte a seguir uma pequena história apenas com emojis 😉, sobre a :cityscape: que escolheu. 
    2. Coloque uma barra horizontal de separação <hr> 
    3. Conte a história por palavras suas. Use etiquetas de estilo e organizacionais para formatar cada palavra diferentemente.
    4. Coloque uma barra horizontal de separação <hr> 
    5. Conte a história por palavras suas sem formatação. 
3. De seguida num novo parágrafo apresente o seu website, criando uma lista não numerada onde apresenta em poucas palavras cada uma das páginas do seu website, incluindo um link para essa página numa das palavras.
4. Criede seguida uma [wordcloud](https://www.wordclouds.com/) com base em palavras que associa à cidade. Adicione as palaras em "wordlist" (apague primeiro as existentes). Ponha peso 10 no nome da cidade para que esta fique com maior destaque. Pode escolher uma forma (shape), fonte (font), cores (use um fundo branco). Descarregue a imagem, e formate-a com o Paint por forma a que tenha largura de 300px como a fotografia da cidade. Isira-a por debaixo da lista.

# 6. Página Localização

Na página `local.html`:
1. Insira um pequeno parágrafo que descreva a localização da ciadade (continente, país), assim como algumas informações geográficas destas.
2.	Insira por baixo um mapa do Google Maps do lugar. Para tal: 
    a. procure o lugar no website www.google.pt/maps
    b. Faça um zoom que considera apropriado
    c. clique em “partilhar” e na opção “incorporar mapa” 
    d. Selecione tamanho pequeno
    e. copie o código HTML resultante, <iframe src=… >
    f. insira esse código HTML na sua pagina HTML.


# 5. Página Multimédia

Na página `multimedia.html`:
1.	Insira um parágrafo que apresente duas fotografias que escolherá no Google por serem emblemáticas do lugar que escolheu.  	 	 
2. Utilize a aplicação Paint ou Paint.Net para gravar duas versões de tamanhos diferentes de cada fotografia (os comandos Ctrl+W ou Ctrl+R permitem abrir um interface que permite configurar o tamanho das imagens, consoante a aplicação): 
    1. Grande, de 800 pixels de largura. Altere o nome, incluindo _grande no fim (e.g., lisboa_grande.jpg).
    2. Pequena, de 100 pixels de largura. Altere o nome, incluindo _pequena (e.g., lisboa_pequena.jpg).
    3. Guarde as 4 fotografias na pasta imagens. 
    4. Insira na página HTML as imagens de 100px de largura, cada uma dentro de um elemento `picture`, incluindo uma legenda descritiva da fotografia (`caption`). Inclua também em cada imagem um hiperlink para a fotografia grande.
3. Pesquise no Youtube um video sobre a cidade escolhida e insira-o na sua página recorrendo à opção "partilhar" e escolhendo "embeded".
4.	Escolha um poema que de alguma forma associa ao lugar escolhido. Escreva, usando tamanhos diferentes, o título numa linha, o nome do poeta na seguinte, seguindo-se o poema, em itálico. Todo o texto deverá estar centrado. 


# 6. Página Informações

Na página `info.html`:
1.	Crie uma tabela com dados à sua escolha sobre a cidade escolhida. Deverá ter pelo menos 3 colunas e 4 colunas. Uma sugestão é ir à wikipedia e extrair alguns elementos que aparecem numa tabela à direita. A terceira coluna pode consistir num elemento agrupador (por exemplo demografia, geografia, história, etc). 
![](lisboa-info.png)
3.	Deve depois formatar esta tabela usando:
    * elementos thead, tfooter e tbody
    * pelo menos um atributo rowspan e um coslpan (o valor de cada um sendo maior que 1). 
    * atributos cellspacing, cellpadding, bgcolor, align, border
    * formatação de colunas com colgroup, explorando os atributos existentes
 


## Lab 2
Crie uma pasta `lab2` com o ficheiro `index.html` que deverá satisfazer os seguintes requisitos:
1. deverá ter como título laboratório 2. 
1. Deverá especificar esse título no `body`, numa etiqueta `h1`.
2. deverá listar os exercícios realizados, com links para os respetivas páginas HTML.
3. deverá ter um link para voltar para a landingpage da sua aplicação no Heroku.

![](wordcloud.png)

Uma vez editado, abra o ficheiro `index.html` com um Browser para ver se visualiza corretamente a imagem em baixo.
![](index-renderizado.png)

## Criação de repositório GitHub
Crie um repositório no GitHub `pw-lab1`, e faça push da pasta `lab1`.

## Alojamento no Heroku
Crie uma conta no Heroku. Sincronize o GitHub com o Heroku, de forma a colocar disponível na cloud a pasta `lab1` com seus conteúdos. 
De forma a conseguirem o alojamento na cloud com sucesso devem seguir os seguintes passos:
* Adicionar dois ficheiros na diretoria `root` da pasta
* * index.php
* * * Com o seguinte conteúdo: `<?php include_once("index.html")  ?>`
* * composer.json
* * * Com o seguinte conteúdo: `{}`
* Criar conta no Heroku - https://signup.heroku.com/login 
* Criar uma aplicação, atribuindo-lhe um nome
* Entrar nas definições da aplicação criada, e clicar na tab `Deploy`
* Na secção de `Deploy Method` devem conectar a aplicação com o Github
* Navegando até ao fim da página, até à secção `Manual deploy`, devem escolher o branch indicado do repositório e clicar em `Deploy branch`
* Um vez realizado com sucesso, devem clicar no botão `Open app` no topo da página, e visualizar a página HTML 


# 2. Conhecer a Internet

Vamos explorar alguns aspectos da Internet, a rede de routers e cabos que suporta Web. 

## Endereços IP
1. Obtenha informação sobre o IP do seu PC e seu telemóvel.
    * obtenha e anote o endereço IP do seu computador. Pode obter isso de várias formas. A mais simples é perguntar no Google "what is my ip". Anote onde está localizado, usando por exemplo a ferramenta https://whatismyipaddress.com/ip-lookup. guarde uma imagem do mapa que localiza.
    * Obtenha e anote a mesma informação do seu telemóvel, se tiver dados móveis.
1. Obtenha informação sobre o IP do servidor Heroku onde está a sua app.
    * Obtenha e anote o endereço IP do servidor Web onde está alojada a sua página no Heroku
    * anote onde este está localizado, usando a ferramenta https://whatismyipaddress.com/ip-lookup.  Guarde uma imagem do mapa que a localiza.

## Percurso
Traceroute (comando tracert) é uma ferramenta de diagnóstico que rastreia a rota que os pacotes IP fazem, desde o seu computador até um endereço IP destino/ou URL que especifique. Este identifica os routers pelos quais os pacotes passam até o seu destino, indicando o tempo que demoram por "salto" entre router. 

1. A forma mais clássica é através da linha de comando e escreva tracert e especifique o endereço IP obtido anteriormente:
``> traceroute <endereço IP ou URL sua app>``
1. Use a ferramenta GeoTraceroute, Em https://geotraceroute.com/, para visualizar graficamente por onde passam os pacotes IP, até chegar ao seu servidor Heroku. Escolha como origem (source) Portugal, e como destino o URL do seu site. Registe os saltos, indicando o país, e distância de cada salto. Quando fizer a página, pode procurar na Internet e inserir uma pequena image da bandeira do país. Com a ferramenta de Snip (Tecla Windows + Shift + S) copie a imagem do globo que cubra os saltos dados, e guarde-a como um ficheiro jpg ou png, para inserir também na página report.html.

# 3. Acesso via HTTP à minha página Web

## HTTP

O protocolo de troca de mensagens entre um cliente e um servidor Web é o HTTP. Um Web browser (Chrome, Safari, Firefox, etc) é uma aplicação que corre numa máquina "cliente" (o seu portátil por exemplo) e é capaz de enviar um pedido usando o protocolo HTTP a um servidor Web:
* O cliente pode pedir uma determinada página Web através de uma mensagem HTTP GET. O servidor Web irá responder-lhe a esse pedido, enviando os conteúdos correspondentes. Tipicamente é recebido um ficheiro HTML juntamente com algumas imagens e outros ficheiros auxiliares, sendo o browser capaz de representar visualmente o conteúdo. 
* O cliente pode também enviar ao servidor Web dados que preencheu por exemplo num formulário, através de uma mensagem HTTP POST. 
Esta é a arquitetura cliente-servidor. 

No seu browser, insira o URL da sua página Heroku. Nesse instante será feito enviado ao servidor Web um pedido (a mensagem chama-se mensagem HTTP GET) do conteúdo correspondente a esse URL, que lhe será enviado pelo servidor em modo de resposta. Visualise o código recebido, clicando com o botão direito do rato e selecionando "ver código fonte" (view page source) ou simplesmente premindo Ctrl + U. Verifique o que aparece: é o que escreveu!

## Inspect

Todos os browsers têm uma ferramenta (*browser developer tool*) que permite inspeccionar ficheiros descarregados pelo browser, permitindo analisar uma grande variedade de informação.
USe por exemplo o Chrome para abrir a sua página, e clicando no botão direito do rato, selecione *Inspect*, ou selecione Ctrl+Shift+i.

Selecione a barra network. Clique na janela  do seu browser onde está o URL do seu site e faça novamente Enter: 
* Explique o que aparece. Com a ferramenta de Snip (Tecla Windows + Shift + S) copie a imagem com info dos ficheiros descarregados. 
* Anote quantos ficheiros são descarregados na sequencia de um clique num hiperlink.
* Anote o tipo de ficheiros, timings de espera e de descarga.
* Selecione cada um dos ficheiros descarregados. Anote o que observa, quando seleciona:
   * preview
   * Headers
   * Timing

Faça o mesmo agora para o site da lusófona, mas aqui observando apenas (sem necessidade de anotar, pois a quantidade de informação é muito maior :-)).

# 4. Página Web Report.html

Com base em todas estas observações crie uma nova página HTML, report.html, onde reporte tudo o que observou.
* Utilize etiquetas para estruturar o seu conteúdo, etiquetas de heading (h1, h2, h3, ....), assim como para listar (ul) e enumerar (ol) (pesquise na internet, nna W3Schools, por exemplo https://www.w3schools.com/tags/tag_ul.asp).
* Inclua as imagens recolhidas da mesma forma que fez no index.html. 
* Faça upload para o seu repositório no GitHub, e sincronize com o Heroku. 
* Verifique que ambas as páginas estão operacionais.

A estrutura das pastas deverá ser como em baixo (com mais imagens na pasta img):
```
projeto
+-- lab1
|   +-- index.html
|   +-- report.html
|   +-- img
    |   +-- wordcloud.png
```

# 5. Submissão do Laboratório
No Moodle, submeta o link da sua aplicação antes da sua próxima aula prática, onde este será avaliado. 

Esperamos que tenha gostado de conhecer um pouco do funcionamento da Internet e de ter feito a sua primeira página Web &#127760;!
