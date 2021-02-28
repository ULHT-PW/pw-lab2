**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**
 
# Programação Web - Laboratório 2: Explorando o HTML com o meu primeiro website  

## Objetivo
* Neste laboratório criará um website sobre uma cidade à sua escolha, onde irá aplicar os conceitos aprendidos sobre HTML.
* Este laboratório deverá ser concluido antes da sua aula prática da semana de 1 de março. Este será avaliado nessa aula. 

## Recomendações
* Leia o enunciado todo com atenção antes de o começar a resolver para entender o que fará.
* Execute com atenção cada passo, certificando-se que implementa todos os detalhes. Contém todos os detalhes para a criação do website. 
* Se tiver alguma dúvida, recorra aos [slides](https://secure.grupolusofona.pt/ulht/moodle/pluginfile.php/958388/mod_resource/content/3/pw-02-html-01.pdf) da aula que contêm todos os conhecimentos que precisa para realizar o laboratório.

## Pré-requisitos
* Instale o VS Code para editar o código HTML de forma fácil.
* Deverá ter feito o [lab1](https://github.com/ULHT-PW-2020-21/pw-lab1).
* Verifique se tem tem instalado o github no seu computador. Para tal, abra uma linha de comando (tecla Windows e escreva cmd) e escreva `git --version`. Caso não o tenha instalado:
    1. aceda à página [Git](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Instalando-o-Git) e siga os passos, mediante o seu sistema operativo (Mac, Linux ou Windows). Para Windows, descarregue diretamente [daqui](https://git-scm.com/download/win) e instale a aplicação descarregada (diga sim em todos os passos de instalação).
    2. uma vez instalado, abra uma janela de comando e execute os seguintes comandos para definir a sua identidade para o git (crie um username, especificando-o entre aspas no comando em baixo, assim como o seu email):
        * `git config --global user.name "username_usado_no_git"`
        * `git config --global user.email "omeu@email.com"`


# 1. Estruturação do repositório de laboratórios
1. O repositório que criou na aula passada albergará todos os laboratórios que fizer em Programação Web. Assim vamos renomeá-lo para um nome mais adequado da seguinte forma:
    1. Abra o seu repositório no GitHub criado na última aula, `pw-lab1`.
    2. Escolha na barra de menú a opção *Settings* 
    3. renomeie o repositório para `pw-labs-nomeapelido-numero` (exemplo: pw-labs-luciostuder-a219999999).  

2. Clone  (descarregue uma cópia) o seu repositório no seu computador local da seguinte forma:
    1. abra um processador de comandos (Tecla Windows e escreva `cmd`, ou `Powershell`, ou `git bash`)
    2. escolha a pasta onde quer colocar o repositório (navegando com o comando `cd nome-de-pasta` para entrar numa determinada pasta)
    3. escreva o comando `git clone https://github/seuusername/pw-labs-nomeapelido-numero` (hiperlink do seu repositório, com o seu username do GitHub e nome do repositório).

3. Na sua pasta `pw-labs-nomeapelido-numero` crie um ficheiro `index.html` que tenha:
    * título "PW Labs" (usando a etiqueta `<title>` no `<head>`)
    * cabeçalho `<h1>` a dizer "Laboratórios Programação Web" 
    * lista com os ítems em baixo, onde a palavra Laboratório x deverá ter um hiperlink para os ficheiros `lab1/index.html` e `lab2/index.html`:
        * Laboratório 1: Conhecer a Internet com a minha primeira página Web
        * Laboratório 2: Explorando o HTML com o meu primeiro website
        
4. Na pasta `lab1` altere o nome do ficheiro `index.html` para  `pw.html`
5. Na pasta `lab1` crie um novo ficheiro `index.html` que tenha:
    * título "PW Lab1" (usando a etiqueta `<title>` no `<head>`)
    * elemento `h1` a dizer "Lab1: Conhecer a Internet com a minha primeira página Web" 
    * lista com os ítems em baixo, onde cada um terá um hiperlink para o respetivo ficheiro (link para `pw.html` e `report.html`):
        * Introdução à programação Web 
        * Conhecer a Internet

6. Crie a pasta `lab2`

7. A estrutura da sua pasta `pw-labs-nomeapelido-numero` deverá ser como em baixo:
```
pw-labs-nomeapelido-numero
+-- index.php
+-- composer.json
+-- index.html
+-- lab1
|   +-- index.html
|   +-- report.html
|   +-- pw.html
|   +-- img
    |   +-- wordcloud.png
    |   +--  ...
+-- lab2
```

8. Abra o ficheiro `index.html` na pasta clonada `pw-labs-nomeapelido-numero`. Verifique que os hiperlinks para o lab1 e das páginas criadas no lab1 funcionam devidamente. O link para lab2 ainda não funciona pois a pasta ainda se encontra vazia.

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
    2. nome do autor do site, descrição do conteudo do site, e palavras chave: 
        * `<meta name="author" content="Ana Maria">`
        * `<meta name="keywords" content="palavras chave">`
        * `<meta name="description" content="Website sobre Lisboa">`

3. Crie um icon para o seu website. Para tal:
    1. Escolha uma imagem que converterá para icon (extensão .ico) recorrendo a uma aplicação web (e.g., https://www.favicon-generator.org/). Alternativamente, pode escolher um icon aqui https://www.iconspedia.com/.
    2. Guarde o icon numa nova pasta `images`, dentro de `lab2`. Garanta que tem a extensão `.ico`
    3. Insira um link para o icon no head da seguinte forma `< link rel="shortcut icon" type="image/x-icon" href="images/favicon.ico"/>`
    4. Poderá observar que, pelo facto de o icon estar na pasta `imagens`, tem sempre que especificar no href o caminho relativo para o local onde se encontra a imagem, o nome da pasta imagens (href="images/imagem.ico”).

4. Explore o site https://www.rapidtables.com/web/color/, onde para cada cor existe uma palete de intensidades que pode escolher. Neste site, escolha uma cor clara para o fundo da sua página, e especifique-a na etiqueta `body` da seguinte forma: `<body style="background-color:plum">` 

# 3. Criação do cabeçalho

Crie agora o cabeçalho do seu website. Terá o nome da Cidade, uma imagem e o menu, ficando da seguinte forma:

![](cabecalho.png)

Para, tal, siga os seguintes passos: 
1.	No body, insira um elemento `h1` com o nome da cidade.
2.	Na linha seguinte insira uma imagem da cidade a seu gosto. Redimensione a imagem para que tenha 300px de largura.No Paint existe uma opção resize que lhe permite escolher o número de pixels que pretende que tenha de largura. Respeite a proporção da imagem, sem a deformar! Guarde a imagem numa nova pasta `images`. Insira a imagem usando a etiqueta `img`. 
3.	Deverá inserir, depois da imagem, uma quebra de linha, `br`, pois o elemento `img` não introduz uma quebra.
4. Irá agora criar o menu. Para tal:
    1. Crie cinco etiquetas de hiperlink `a`, tendo como conteúdo o nome das páginas do seu site (Introdução, Localização, Multimédia, Informações, Home), estando os elementos separados pelo carater `|`. 
    2. Use como valor para o atributo `href` as seguintes páginas:
        1. `index.html` para Introdução 
        2. `local.html` para Localização
        3. `multimedia.html` para Multimédia
        4. `info.html` para Informações
        5. `../index.html` para Home (indice geral dos laboratórios)

# 4. Criação das páginas do website

De seguida iremos criar as páginas do seu website que estarão interligadas.
1.	Crie 4 copias do ficheiro index.html que criou. 
2.	Altere os nomes dos ficheiros para ter um de cada, com os seguintes nomes: index.html, local.html, multimedia.html, info.html (atenção que os nomes dos ficheiros HTML  deverão estar em minúsculas, sem espaços, acentos ou carateres especiais)
3.	Em cada ficheiro, no menu ponha a negrito a palavra a que corresponde a página.
4.	Abra o ficheiro index, e experimente se os hiperlinks funcionam. 
Tem agora criado o seu website! Agora irá preencher cada página com conteúdos.

# 5. Página Introdução

Na pagina `index.html` insira, no body, por debaixo do menu:
1. Um elemento `h3` com a palavra Introdução.
2. um parágrafo sobre esta cidade.
3. Pesquise na Internet por [carateres especiais UTF-8](https://www.w3schools.com/charsets/ref_html_utf8.asp) assim como por emojis na [W3Schools](https://www.w3schools.com/charsets/ref_emoji.asp) e na [emojipedia](https://emojipedia.org/): 
    1. Conte a seguir uma pequena história apenas com emojis 😉, sobre a :cityscape: que escolheu. 
    2. Coloque uma barra horizontal de separação `hr` 
    3. Conte a história por palavras suas. Use etiquetas de estilo e organizacionais para formatar cada palavra diferentemente.
    4. Coloque uma barra horizontal de separação `hr` 
    5. Conte a história por palavras suas sem formatação. 
4. De seguida num novo parágrafo apresente o seu website, criando uma lista não numerada onde apresenta em poucas palavras cada uma das páginas do seu website, incluindo um link para essa página numa das palavras.
5. Crie de seguida uma [wordcloud](https://www.wordclouds.com/) com base em palavras que associa à cidade. Adicione as palaras em "wordlist" (apague primeiro as existentes). Ponha peso 10 no nome da cidade para que esta fique com maior destaque. Pode escolher uma forma (shape), fonte (font), cores (use um fundo branco). Descarregue a imagem, e formate-a com o Paint por forma a que tenha largura de 300px como a fotografia da cidade. Isira-a por debaixo da lista.

# 6. Página Localização

Na página `local.html`:
1. Um elemento `h3` com a palavra Localização.
2. Insira um pequeno parágrafo que descreva a localização da ciadade (continente, país), assim como algumas informações geográficas destas.
3.	Insira por baixo um mapa do Google Maps do lugar. Para tal: 
    a. procure o lugar no website www.google.pt/maps
    b. Faça um zoom que considera apropriado
    c. clique em “partilhar” e na opção “incorporar mapa” 
    d. Selecione tamanho pequeno
    e. copie o código HTML resultante, `<iframe src=… >`
    f. insira esse código HTML na sua pagina HTML
    g. acerte a dimensão da janela.


# 5. Página Multimédia

Na página `multimedia.html`:
1. Um elemento `h3` com a palavra Multimédia.
2.	Insira um parágrafo que apresente duas fotografias que escolherá no Google por serem emblemáticas do lugar que escolheu.  	 	 
3. Utilize a aplicação Paint ou Paint.Net para gravar duas versões de tamanhos diferentes de cada fotografia (os comandos Ctrl+W ou Ctrl+R permitem abrir um interface que permite configurar o tamanho das imagens, consoante a aplicação): 
    1. Grande, de 800 pixels de largura. Altere o nome, incluindo _grande no fim (e.g., lisboa_grande.jpg).
    2. Pequena, de 100 pixels de largura. Altere o nome, incluindo _pequena (e.g., lisboa_pequena.jpg).
    3. Guarde as 4 fotografias na pasta `imagens`. 
    4. Insira na página HTML as imagens de 100px de largura, cada uma dentro de um elemento `picture`, incluindo uma legenda descritiva da fotografia (`caption`).  Especifique o campo `alt`. Aninhe o elemento `img` dentro de um hiperlink `a`, com hiperligação para a fotografia grande correspondente. No hiperlink, especifique o atributo `target="_blank"`, para que a imagem abra numa nova janela de forma isolada (ficará de forma primária, mas para este laboratório é suficiente).
4. Pesquise no Youtube um video sobre a cidade escolhida e insira-o na sua página recorrendo à opção "partilhar" e escolhendo "embeded".
5.	Escolha um poema que de alguma forma associa ao lugar escolhido. Escreva, usando tamanhos diferentes, o título numa linha, o nome do poeta na seguinte, seguindo-se o poema, em itálico. Todo o texto deverá estar centrado. 


# 6. Página Informações

Na página `info.html`:
1.	Um elemento `h3` com a palavra Informações.
2. Crie uma frase a introduzir uma tabela de informações a compilar sobre a cidade.	
3.	Crie uma tabela com dados à sua escolha sobre a cidade escolhida. Deverá ter pelo menos 3 colunas e 4 colunas. Uma sugestão é ir à wikipedia e extrair alguns elementos que aparecem numa tabela à direita. A terceira coluna pode consistir num elemento agrupador (por exemplo demografia, geografia, história, etc). Exemplo de tabela:

    ![](lisboa-info.png)

4.	Deve depois formatar esta tabela usando os seguintes atributos:
    * pelo menos um atributo rowspan e um coslpan (o valor de cada um sendo maior que 1). 
    * cellspacing,
    * cellpadding, 
    * bgcolor, 
    * align, 
    * border (use border="1"),
    * formatação de colunas com colgroup, explorando os atributos existentes

# 7. Submissão

A estrutura final da sua pasta `pw-labs-nomeapelido-numero` deverá ser como em baixo:
```
`pw-labs-nomeapelido-numero`
+-- index.php
+-- composer.json
+-- index.html
+-- lab1
|   +-- index.html
|   +-- report.html
|   +-- pw.html
|   +-- img
    |   +-- wordcloud.png
    |   +--  ...
+-- lab2
|   +-- index.html
|   +-- info.html
|   +-- local.html
|   +-- multimedia.html
|   +-- images
    |   +--  ...
```

1. Antes de submeter, verifique que todos os links funcionam devidamente.
2. Carregue a sua pasta no Github com as seguintes instruções: 
    1.  abra o processador de comandos e posicione-se dentro da pasta do seu repositório (`pw-labs-nomeapelido-numero`).
    2.  escreva as seguintes instruções:
        * `git add *`
        * `git commit –m "submissão laboratório 2"`
        * `git push`
3. Sincronize o GitHub com o Heroku tal como fez no [lab1](https://github.com/ULHT-PW-2020-21/pw-lab1). Deverá ir ao Heroku e, em Deploy, fazer deploy branch, de forma a colocar disponível na cloud os novos conteúdos criados. 
4. Garanta que o link da sua aplicação se encontra [aqui](https://drive.google.com/file/d/1kphRYAo78NSxWznBXHqNbPksELqlyloI/view). Inclua também o hiperlink do seu repositório privado no GitHub, e adicione os docentes de PW como membros, que têm como usernames no GitHub: luciostuder, logdarkmatter, rfgsantos. Finalize o laboratório antes da sua próxima aula prática, onde este será avaliado. 

Esperamos que tenha gostado de aplicar os conhecimentos de HTML e de ter feito um website &#127760;!
