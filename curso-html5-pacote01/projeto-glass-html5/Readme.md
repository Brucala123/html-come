          ESTUDO HTML
-------------------------------------
-Estilo padrao de html

=======================================
<DOCTYPE html>
<html lang = "pt-br">
    <head>
        <meta charset = "UTF-8">
        <meta name="viewport" content="width-device-width; initial-scale=1.0">
    </head>
<body>



</body>
</html>
()<style> : usada por conta do css para alterar o visual do site(posto entre o head) 
()font-family : altera do tipo do texto ou fonte
()font-size : altera o tamanho do texto
()color : altera a cor do texto
()text-shadow (deslocamento lateral) [tamanho em pixel] (deslocamento vertical)[tamanho em pixel] (espalhamento da sombra)[tamanho em pixel] [cor] : coloca uma sombra na escrita
=========================
<div> divisoria para facilitar a edicao no css
<hgroup> agrupa textos
<img src =""> inserir imagem
<header> cabecalho (outra div)

==============
<br> - quebra de linha
&nbsp - espaco sem quebra
<p> texto ou paragrafo
<wbr/> quebra de palavra
&shy; soft hyphen

===================
    SIMBOLOS

&lt; <
&gt; >
&le; <=
&ge; >=

-----------

&pound;
&yen;
&euro;

-------------

&copy;
&reg;
&trade;

---------

&permil; /1000
&sum;
&infin;
&times;
&plusmn;
&oplus;
&radic;
&ne;

------------

&delta; &Delta;
&lambda;
&omega;
&phi;

-----------

&larr;
&rarr; &Rarr;
&uarr;
&darr;
&harr;

----------

&spades;
&clubs;
&hearts;
&diams;


formatações:

<pre> todos os espaços e enters serão considerados
<code> codigo - formata como em fonte de codigo
<sub> subescrito - escreve embaixo
<sup> supreescrito -  como se fosse elevado 
<b> bold - coloca em negrito as palavras
<i> italico - coloca em italico as palavras
<em> enfase - parecido com o italico
<u> underline - sublinha
<del> risca - risca a palavra por cima
<span> usada para formatar pequenos trechos de texto, podendo assim fazer <span style = "text-decoration: underline;"> ou overline, line-through e o none
<span style = "font-weight: normal;"> ou bold, bolder ou colocar um valor entre 100-900
Ter edições em separações de titulos, h1, como por exemplo:
<h2 style = "text-align: center;"> ou left ou right
<p style = "text-align: justify; text indent: 50px;> - coloca o paragrafo direito


Para faazer isso de mandeira global, basta colocar em "head" o <style></style>, dentre eles vc coloca tudo que for de CSS

Exemplo: 
    <style>
            p{
                text-align: justify;
                text-indent: 50px;
            }
        </style>

Edição de cores:
(vermelho, verde, azul)
hsl(x,x,x)
hsla(x,x,x,x)
rgb(x,x,x)
rgba(x,x,x,x)
hecadecimal: #192304

ou colocar também imagens de fundo:
url("")


Mudar o tamanho da imagem para o site ficar mais leve

<figure> - usado para agrupar imagem e dar um significado semantico a elas
<figcaption> - legenda para imagem
exemplo:

<figure>
        [codigo de imagem]
    <figcaption>
        <h3>Olá!</h3>
    </figcaption>
</figure>


COLOCAR O ESTILO (CSS) EM OUTRA PASTA: 

@charset "UTF-8";

[Codigo]

No arquivo com html para fazer a ligação:

rel = stylesheet - folha de estilo
type = text/css
href - hypertext reference, ele chama um arquivo de fora

<link rel="stylesheet" type="text/css" href="_css/estilo.css">


SEMPRE QUE UTILIZAR O PARAMETRO "CLASS", ELE VAI SER ESCRITO ASSIM NO CSS:

figure.foto-legenda{

}

DENTRO DO PARAMETRO PODES QUERER EDITAR ALGO ESPECIFICO, PODENDO ASSIM: 

figure.foto-legenda img {

}

box-shadow:1px 1px 4px black;


Codigo:
NESTE CODIGO O "RELATIVE" TEM FUNÇÃO DE SER BASEADO NA POSIÇÃO QUE O FIGURE ESTÁ, FAZENDO O "ABSOLUTE" DO FIGCAPTION SER DENTRO DO CONTAINER DO FIGURE:


figure.foto-legenda{
    position: relative;
    border: 8px solid white;
    box-shadow: 1px 1px 4px black;
}
figure.foto-legenda img{
    width: 100%;
    height: 100%;
}
figure.foto-legenda figcaption{
    position: absolute;
    top: 0px;
}

padding: 10px; - muda o espaço dentro da legenda, aumentando a legenda ou diminuindo

box-sizing: ; - cria um box dentro da borda

opacity: ; - o quao é visível a legenda


----------------------------------
O "hover" vai fzer com que exerça uma formatação expecifica quando o mouse passar em cima do objeto


figure.foto-legenda:hover figcaption{

}

transition: opacity 1s; - faz com que tenha uma transição de 1s na opacidade



<nav> - cria um container de navegação

transformar itens em lista:
dentro de cada uma das listas tem o:

list items - li
------------------

Ordered list - ol:
tipos de listas ordenadas - 
+ type = "1"
+ type = "a"
+ type = "i"
(para começar com outro numero ou letra tem o comando: start = "[numero]")
-----------------

unordered list - ul:
tipos de listas nao ordenadas:
+ type = "square"
+ type = "circle"
+ type = "disc"


