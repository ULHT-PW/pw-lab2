**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**
 
# Programação Web - Laboratório 2: Explorando o HTML com o meu primeiro website  

## Objetivo
* Neste laboratório criará um website sobre uma cidade à sua escolha, onde irá aplicar os conceitos aprendidos sobre HTML.

## Pré-requisitos
* Instale o VS Code para editar o código HTML de forma fácil.
* Deverá ter feito o [lab1](https://github.com/ULHT-PW-2020-21/pw-lab1).
* Leia o enunciado todo antes de o começar a resolver para entender o que fará.

## Nota
* Deverá concluir o laboratório antes da sua aula prática da semana de 1 de março. Este será avaliado nessa aula. 

# 1. Estruturação

1. Na sua pasta `projeto` (que se encontra no GitHub) crie o ficheiro `index.html` que:
    * tenha como título "Laboratórios Programação Web" (etiqueta `<title>`)
    * tenha um cabeçalho `<h1>` a dizer "Laboratórios Programação Web" 
    * deverá ter, numa lista, os nomes dos labs 1 e 2 ("Laboratório 1: Conhecer a Internet com a minha primeira página Web" e  "Laboratório 2: Explorando o HTML com o meu primeiro website"), cada um respetivamente com links para os ficheiros `lab1/lab1.html` e `lab2/index.html`.
2. Na pasta `lab1` crie o ficheiro `lab1.html` que:
    * tenha como título "lab1" (usando a etiqueta `<title>` no `<<head>`)
    * tenha um elemento `h1` a dizer "Lab1: Conhecer a Internet com a minha primeira página Web" 
    * tenha, numa lista, com os seguintes items:
        * link para `index.html`.
        * link para `report.html`. 
2. crie a pasta `lab2`

# 2. Página Web 

Fará neste laboratório 2 um website sobre uma cidade do mundo à sua escolha que goste. Deverá congregar várias informações sobre esta conforme indicado ao longo do laboratório. 

Na pasta `lab2` crie o ficheiro `index.html`, inserindo as partes elementares:

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
    2. Guarde-o numa nova pasta `imagens`, dentro de `lab2`
    3. Insira um link para o icon no head da seguinte forma `< link rel="shortcut icon" type="image/x-icon" href="imagens/favicon.ico"/>`
    4. Poderá observar que, pelo facto de o icon estar na pasta `imagens`, tem sempre que especificar no href o caminho relativo para o local onde se encontra a imagem, o nome da pasta imagens (href="imagens/imagem.ico”).

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
    2. Coloque uma barra horizontal de separação `hr` 
    3. Conte a história por palavras suas. Use etiquetas de estilo e organizacionais para formatar cada palavra diferentemente.
    4. Coloque uma barra horizontal de separação `hr` 
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
    e. copie o código HTML resultante, `<iframe src=… >`
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
1.	Crie uma frase a introduzir a tabela de informações que compilou sobre a cidade.
2.	Crie uma tabela com dados à sua escolha sobre a cidade escolhida. Deverá ter pelo menos 3 colunas e 4 colunas. Uma sugestão é ir à wikipedia e extrair alguns elementos que aparecem numa tabela à direita. A terceira coluna pode consistir num elemento agrupador (por exemplo demografia, geografia, história, etc). Exemplo de tabela:

    ![](lisboa-info.png)

3.	Deve depois formatar esta tabela usando:
    * pelo menos um atributo rowspan e um coslpan (o valor de cada um sendo maior que 1). 
    * atributos cellspacing, cellpadding, bgcolor, align, border
    * formatação de colunas com colgroup, explorando os atributos existentes

# 7. Submissão

A estrutura final da sua pasta `repo`, o seu repositório público do GitHub, deverá ser como em baixo:
```
repo
+-- index.php
+-- composer.json
+-- index.html
+-- lab1
|   +-- lab1.html
|   +-- index.html
|   +-- report.html
|   +-- img
    |   +-- wordcloud.png
    |   +--  ...
+-- lab2
|   +-- index.html
|   +-- info.html
|   +-- local.html
|   +-- multimedia.html
|   +-- imagens
    |   +--  ...
```

1. Faça commit e push da pasta `projeto` para o seu repositório `pw-lab1`. Poderá se quiser renomear esta pasta para `pw-labs` pois este repositório irá conter todos os laboratórios que fizer em Programação Web.
2. Sincronize o GitHub com o Heroku tal como fez no [lab1](https://github.com/ULHT-PW-2020-21/pw-lab1), de forma a colocar disponível na cloud a pasta `projeto` com seus conteúdos. 
3. Garanta que o link da sua aplicação se encontra [aqui](https://drive.google.com/file/d/1kphRYAo78NSxWznBXHqNbPksELqlyloI/view). Finalize o laboratório antes da sua próxima aula prática, onde este será avaliado. 

Esperamos que tenha gostado de aplicar os conhecimentos de HTML e de ter feito um website &#127760;!
