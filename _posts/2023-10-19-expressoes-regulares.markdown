---
layout: post
title:  "Expressões Regulares"
date:   2023-10-19 19:23:00 -0300
categories: jekyll update
---

__*Expressão regular:*__ Método formal de especificar um padrão de texto.

__*Metacaracteres:*__ Conjunto de símbolos e caracteres literais usados como elementos constituintes de uma expressão regular.


Metacaractere   |   Nome    |   Tipo    |   Função
:---------:     |   ------  |   ------  |   ------
.       | Ponto         |   Representante   |   Um caractere Qualquer
[...]   | Lista         |   Representante   |   Uma lista de cracteres permitidos
[^...]  | Lista negada  |   Representante   |   Uma lista de caracteres proibidos
?       | Opcional      |   Quantificadores |   Zero ou um
\*      | Asterisco     |   Quantificadores |   Zero, um ou mais
\+      | Mais          |   Quantificadores |   Um ou mais
{n,m}   | Chaves        |   Quantificadores |   De n até m
^       | Circunflexo   |   Âncoras         |   Inicio de linha 
$       | Cifrão        |   Âncoras         |   Fim de linha
\\b     | Borda         |   Âncoras         |   Inicio ou fim de palavra
\\      | Escape        |   Outros          |   Torna literal o caractere ao seu lado
\|      | Ou            |   Outros          |   Ou um ou outro
\(...)  | Grupo         |   Outros          |   Delimita um grupo
\\1...9 | Retrovisor    |   Outros          |   Texto casado nos grupos 1...9


__*Tipos de Metacaracters:*__

1. Representante: 
Esses metacaracteres representam um ou mais caracteres. Podem ser chamados de "apelidos", por exemplo. Todos os metacaracteres desse tipo casam com a posição de um e somente um caractere. 

2. Quantificadores:
Os quantificadores são usados para indicar a quantidade de repetições permitidas para o elemento imediatamente anterior. Essa entidade pode ser um caractere ou um metacaractere. Em princípio, quantificadores não são "quantificáveis", o que quer dizer que não podemos usar um quantificador seguido do outro. Mas isso é relativo. 😉

3. Âncoras: Como o próprio nome já nos dá uma pista: elas ancoram uma posição específica em uma linha. Quantificadores não têm ação sobre as âncoras. 


4. Outros: Abordaremos esses mais adiante...
