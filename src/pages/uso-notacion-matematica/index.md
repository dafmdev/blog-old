---
title: Uso de notación matemática
date: "2020-11-04T22:12:03.284Z"
spoiler: "Las matemáticas tienen su propio lenguaje, usalo digitalmente en tu blog"
discussionId: "2020-11-04-page-slug2"
---

Las matemáticas tienen su propio lenguaje, así como yo uso el español (lenguaje informal) para trasmitir ciertas ideas en este blog, otras personas usan otros idiomas para comunicarse, los matemáticos y las personas que usan las matemáticas escriben en el lenguaje de las matemáticas, su nombre técnico es [Notación matemática](https://es.wikipedia.org/wiki/Notaci%C3%B3n_matem%C3%A1tica) (lenguaje formal).

Se compone por números, y símbolos que en sí mismos representan un concepto, una relación, una operación. Siguiendo ciertas reglas a la hora de usar estos símbolos, podemos comunicar formalmente una «oración» una fórmula matemática, que puede ser comprendida por alguien más, como guía para su posterior solución. He aquí, la importancia de escribir bien las matemáticas.

Muchos de nosotros estamos en la capacidad de escribir notación matemática a mano, en los colegios nos ponían a realizar muchas sumas, restas, multiplicaciones, divisiones, raíces, etc. Pero ahora tenemos un reto, no estamos escribiendo esta bitácora a mano, estamos usando un medio digital.

Por eso, otras personas del pasado con la necesidad de escribir bien las matemáticas se inventaron un [lenguaje de marcado](https://es.wikipedia.org/wiki/Lenguaje_de_marcado) llamado $\LaTeX$, cuando alguien escribe en este lenguaje de marcado, la computadora podrá entender y renderizar una notación matemática hermosa, que cualquier matemático podrá entender si se usa bien.

## ¿Cómo usar $\LaTeX$?
Hay dos opciones principales, aprender cómo se escribe en este lenguaje de marcado mediante la [documentación](https://es.wikibooks.org/wiki/Manual_de_LaTeX/Texto_completo) que existe en internet, o usar un editor de ecuaciones matemáticas que use LaTeX y de esta forma el software te genera el código LaTeX de forma automática. Yo me iré por esta última opción.

Hay muchas opciones, tanto software de escritorio para descargar o herramientas web. En mi caso, uso 3 paginas que me gustan mucho:

 - [Symbolab](https://es.symbolab.com/])
 - [Codecogs](https://www.codecogs.com/latex/eqneditor.php)
 - [iMathEQ](http://www.imatheq.com/imatheq/com/imatheq/math-equation-editor-latex-mathml.html)

Dentro de estas páginas, lo único que deben hacer, es modelar las expresiones matemáticas como lo harían a mano y posteriormente la propia página web les dará el código en formato $\LaTeX$.

## ¿Qué hago con este código?
El código de marcado de LaTeX se puede pegar en un lugar que lea este formato para representar ecuaciones matemáticas, por ejemplo, Microsoft Word, Notion, LibreOffice, Markdown, Wordpress, Google Colab, Jupyter Notebook, entre muchos otros.

Como pueden ver, tiene mucho respaldo y es muy útil usarlo para dejar los malos hábitos de representar ecuaciones matemáticas en un formato lineal, ejemplo: `2/3+(5*(1-3)^4-5)/(45-10)` esto dificulta mucho al lector entender que se quiere decir y se presta para malas interpretaciones. A diferencias de hacer esto:

$$
\frac{\frac{2}{3}+(5\cdot(1-3)^{4}-5}{45-10}
$$

Esta es una comparación de como se ve una notación matemática lineal y notación matemática clásica:

|Lineal |Código $\LaTeX$|Salida|
|--|--|--|
|2+2|`2+2` |$2 + 2$ |
|2/2=1|`\frac{2}{2}=1` |$\frac{2}{2}=1$ |
|5^2-10=15|`5^{2}-10=15` |$5^{2}-10=15$ |
|raiz(16)*10^5=400000|`\sqrt{16}\cdot10^{5}=400000` |$\sqrt{16}\cdot10^{5}=400000$ |
|No sé|`\sum_{n=0}^{\infty \:}\left(-1\right)^n` |$\sum_{n=0}^{\infty \:}\left(-1\right)^n$|
|No sé|`\begin{pmatrix}1&2&3\\4&5&6\\ 7&8&9\end{pmatrix}` |$\begin{pmatrix}1&2&3\\ 4&5&6\\ 7&8&9\end{pmatrix}$ |

Cómo pueden observar cuando se usa $\LaTeX$, queda mucho más profesional y correcto las ecuaciones matemáticas. Y todo este código no los escribí yo, los hice usando iMathEQ.

También pueden usar estos códigos en Notion, solo deben poner `/`esta barra que indica que van a ingresar un bloque especial y escriben `/latex`, les debe salir algo como esto:

<p><img src="https://i.imgur.com/6dz6GX5.png"></p>

Luego ponen el código en formato LaTeX y Notion automáticamente mostrara la ecuación matemática renderizada así:

<p><img src="https://i.imgur.com/WD7npW9.png"></p>

De esta forma, los apuntes matemáticos serán mucho más claros y de mayor calidad. Ver la matemática bien escrita no solo es bonito da gusto verla.
Les dejo esta [pagina](https://manualdelatex.com/) web, que les podrá servir como diccionario para símbolos especiales en $\LaTeX$. Y esta [otra](https://katex.org/docs/supported.html) en caso de que estén usando Notion para crear la bitácora.
