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
