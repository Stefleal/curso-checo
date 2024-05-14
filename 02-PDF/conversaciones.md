<!DOCTYPE html>
<html>
<head>
<title>conversaciones.md</title>
<meta http-equiv="Content-type" content="text/html;charset=UTF-8">

<style>
/* https://github.com/microsoft/vscode/blob/master/extensions/markdown-language-features/media/markdown.css */
/*---------------------------------------------------------------------------------------------
 *  Copyright (c) Microsoft Corporation. All rights reserved.
 *  Licensed under the MIT License. See License.txt in the project root for license information.
 *--------------------------------------------------------------------------------------------*/

body {
	font-family: var(--vscode-markdown-font-family, -apple-system, BlinkMacSystemFont, "Segoe WPC", "Segoe UI", "Ubuntu", "Droid Sans", sans-serif);
	font-size: var(--vscode-markdown-font-size, 14px);
	padding: 0 26px;
	line-height: var(--vscode-markdown-line-height, 22px);
	word-wrap: break-word;
}

#code-csp-warning {
	position: fixed;
	top: 0;
	right: 0;
	color: white;
	margin: 16px;
	text-align: center;
	font-size: 12px;
	font-family: sans-serif;
	background-color:#444444;
	cursor: pointer;
	padding: 6px;
	box-shadow: 1px 1px 1px rgba(0,0,0,.25);
}

#code-csp-warning:hover {
	text-decoration: none;
	background-color:#007acc;
	box-shadow: 2px 2px 2px rgba(0,0,0,.25);
}

body.scrollBeyondLastLine {
	margin-bottom: calc(100vh - 22px);
}

body.showEditorSelection .code-line {
	position: relative;
}

body.showEditorSelection .code-active-line:before,
body.showEditorSelection .code-line:hover:before {
	content: "";
	display: block;
	position: absolute;
	top: 0;
	left: -12px;
	height: 100%;
}

body.showEditorSelection li.code-active-line:before,
body.showEditorSelection li.code-line:hover:before {
	left: -30px;
}

.vscode-light.showEditorSelection .code-active-line:before {
	border-left: 3px solid rgba(0, 0, 0, 0.15);
}

.vscode-light.showEditorSelection .code-line:hover:before {
	border-left: 3px solid rgba(0, 0, 0, 0.40);
}

.vscode-light.showEditorSelection .code-line .code-line:hover:before {
	border-left: none;
}

.vscode-dark.showEditorSelection .code-active-line:before {
	border-left: 3px solid rgba(255, 255, 255, 0.4);
}

.vscode-dark.showEditorSelection .code-line:hover:before {
	border-left: 3px solid rgba(255, 255, 255, 0.60);
}

.vscode-dark.showEditorSelection .code-line .code-line:hover:before {
	border-left: none;
}

.vscode-high-contrast.showEditorSelection .code-active-line:before {
	border-left: 3px solid rgba(255, 160, 0, 0.7);
}

.vscode-high-contrast.showEditorSelection .code-line:hover:before {
	border-left: 3px solid rgba(255, 160, 0, 1);
}

.vscode-high-contrast.showEditorSelection .code-line .code-line:hover:before {
	border-left: none;
}

img {
	max-width: 100%;
	max-height: 100%;
}

a {
	text-decoration: none;
}

a:hover {
	text-decoration: underline;
}

a:focus,
input:focus,
select:focus,
textarea:focus {
	outline: 1px solid -webkit-focus-ring-color;
	outline-offset: -1px;
}

hr {
	border: 0;
	height: 2px;
	border-bottom: 2px solid;
}

h1 {
	padding-bottom: 0.3em;
	line-height: 1.2;
	border-bottom-width: 1px;
	border-bottom-style: solid;
}

h1, h2, h3 {
	font-weight: normal;
}

table {
	border-collapse: collapse;
}

table > thead > tr > th {
	text-align: left;
	border-bottom: 1px solid;
}

table > thead > tr > th,
table > thead > tr > td,
table > tbody > tr > th,
table > tbody > tr > td {
	padding: 5px 10px;
}

table > tbody > tr + tr > td {
	border-top: 1px solid;
}

blockquote {
	margin: 0 7px 0 5px;
	padding: 0 16px 0 10px;
	border-left-width: 5px;
	border-left-style: solid;
}

code {
	font-family: Menlo, Monaco, Consolas, "Droid Sans Mono", "Courier New", monospace, "Droid Sans Fallback";
	font-size: 1em;
	line-height: 1.357em;
}

body.wordWrap pre {
	white-space: pre-wrap;
}

pre:not(.hljs),
pre.hljs code > div {
	padding: 16px;
	border-radius: 3px;
	overflow: auto;
}

pre code {
	color: var(--vscode-editor-foreground);
	tab-size: 4;
}

/** Theming */

.vscode-light pre {
	background-color: rgba(220, 220, 220, 0.4);
}

.vscode-dark pre {
	background-color: rgba(10, 10, 10, 0.4);
}

.vscode-high-contrast pre {
	background-color: rgb(0, 0, 0);
}

.vscode-high-contrast h1 {
	border-color: rgb(0, 0, 0);
}

.vscode-light table > thead > tr > th {
	border-color: rgba(0, 0, 0, 0.69);
}

.vscode-dark table > thead > tr > th {
	border-color: rgba(255, 255, 255, 0.69);
}

.vscode-light h1,
.vscode-light hr,
.vscode-light table > tbody > tr + tr > td {
	border-color: rgba(0, 0, 0, 0.18);
}

.vscode-dark h1,
.vscode-dark hr,
.vscode-dark table > tbody > tr + tr > td {
	border-color: rgba(255, 255, 255, 0.18);
}

</style>

<style>
/* Tomorrow Theme */
/* http://jmblog.github.com/color-themes-for-google-code-highlightjs */
/* Original theme - https://github.com/chriskempson/tomorrow-theme */

/* Tomorrow Comment */
.hljs-comment,
.hljs-quote {
	color: #8e908c;
}

/* Tomorrow Red */
.hljs-variable,
.hljs-template-variable,
.hljs-tag,
.hljs-name,
.hljs-selector-id,
.hljs-selector-class,
.hljs-regexp,
.hljs-deletion {
	color: #c82829;
}

/* Tomorrow Orange */
.hljs-number,
.hljs-built_in,
.hljs-builtin-name,
.hljs-literal,
.hljs-type,
.hljs-params,
.hljs-meta,
.hljs-link {
	color: #f5871f;
}

/* Tomorrow Yellow */
.hljs-attribute {
	color: #eab700;
}

/* Tomorrow Green */
.hljs-string,
.hljs-symbol,
.hljs-bullet,
.hljs-addition {
	color: #718c00;
}

/* Tomorrow Blue */
.hljs-title,
.hljs-section {
	color: #4271ae;
}

/* Tomorrow Purple */
.hljs-keyword,
.hljs-selector-tag {
	color: #8959a8;
}

.hljs {
	display: block;
	overflow-x: auto;
	color: #4d4d4c;
	padding: 0.5em;
}

.hljs-emphasis {
	font-style: italic;
}

.hljs-strong {
	font-weight: bold;
}
</style>

<style>
/*
 * Markdown PDF CSS
 */

 body {
	font-family: -apple-system, BlinkMacSystemFont, "Segoe WPC", "Segoe UI", "Ubuntu", "Droid Sans", sans-serif, "Meiryo";
	padding: 0 12px;
}

pre {
	background-color: #f8f8f8;
	border: 1px solid #cccccc;
	border-radius: 3px;
	overflow-x: auto;
	white-space: pre-wrap;
	overflow-wrap: break-word;
}

pre:not(.hljs) {
	padding: 23px;
	line-height: 19px;
}

blockquote {
	background: rgba(127, 127, 127, 0.1);
	border-color: rgba(0, 122, 204, 0.5);
}

.emoji {
	height: 1.4em;
}

code {
	font-size: 14px;
	line-height: 19px;
}

/* for inline code */
:not(pre):not(.hljs) > code {
	color: #C9AE75; /* Change the old color so it seems less like an error */
	font-size: inherit;
}

/* Page Break : use <div class="page"/> to insert page break
-------------------------------------------------------- */
.page {
	page-break-after: always;
}

</style>

<script src="https://unpkg.com/mermaid/dist/mermaid.min.js"></script>
</head>
<body>
  <script>
    mermaid.initialize({
      startOnLoad: true,
      theme: document.body.classList.contains('vscode-dark') || document.body.classList.contains('vscode-high-contrast')
          ? 'dark'
          : 'default'
    });
  </script>
<h1 id="%22conversaciones-cotidianas-en-un-idioma-extranjero%22">&quot;Conversaciones cotidianas en un idioma extranjero&quot;</h1>
<p><em>Una historia de preparación con Nino, el minino.</em></p>
<p><img src="ninominino.jpg" alt="Nino"></p>
<h3 id="siempre-quise-salir-de-mi-casa-y-conocer-el-mundo-pero-ya-ven-que-salir-es-cada-vez-m%C3%A1s-dif%C3%ADcil-que-todo-est%C3%A1-caro-que-la-inflaci%C3%B3n-el-cambio-de-gobierno-y-todas-esas-tonter%C3%ADas-que-se-le-ocurren-a-los-humanos">Siempre quise salir de mi casa y conocer el mundo, pero ya ven que salir es cada vez más difícil. Que todo está caro, que la inflación, el cambio de gobierno y todas esas tonterías que se le ocurren a los humanos.</h3>
<h3 id="lo-cierto-es-que-he-visto-un-lugar-al-que-quisiera-ir-kav%C3%A1rna-ko%C4%8Di%C4%8D%C3%AD-prague-no-solo-porque-podr%C3%ADa-andar-libre-sino-porque-es-un-lugar-donde-ning%C3%BAn-animal-sale-herido">Lo cierto es que he visto un lugar al que quisiera ir <a href="http://kavarnakocici.com/">Kavárna Kočičí Prague</a>, no solo porque podría andar libre, sino porque es un lugar donde ningún animal sale herido.</h3>
<h3 id="por-esta-raz%C3%B3n-he-comenzado-a-practicar-el-checo-sisisisisi-ya-s%C3%A9-que-es-un-idioma-complejo-y-que-solo-lo-hablan-all%C3%AD-escuch%C3%A9-a-chenlo-pero-ya-ver%C3%A1n-que-no-ser%C3%A1-tan-dif%C3%ADcil">Por esta razón he comenzado a practicar el checo. Sisisisisi, ya sé que es un idioma complejo y que solo lo hablan allí, <s>escuché a Chenlo</s>, pero ya verán que no será tan difícil.</h3>
<pre class="hljs"><code><div>No sé si les dije, pero mi nombre es Nino, soy un gato de 5 meses y mi tutora es Stefanía, la típica vieja de los gatos.
Me gustan las latitas de comida, correr por la casa y morder a lo loco.

</div></code></pre>
<p><img src="loca-de-los-gatos.gif" alt="loca"></p>
<h3 id="a-continuaci%C3%B3n-te-dejo-un-avance-de-la-unidad-1-de-mi-estudio-por-si-quieres-ir-conmigo-prrr-%C2%A1comencemos">A continuación, te dejo un avance de la <em>Unidad 1</em> de mi estudio, por si quieres ir conmigo, prrr ¡Comencemos!</h3>
<hr>
<h1 id="1-saludos-cotidianos-saludos">1. Saludos cotidianos <img src="patita.jpg" alt="Saludos"></h1>
<blockquote>
<p>Hola! encantado <strong>Ahoj! Velmi rád!</strong></p>
</blockquote>
<blockquote>
<p>¿Qué tal? <strong>Jak se máte?</strong></p>
</blockquote>
<blockquote>
<p>¡Qué lindo gato! <strong>jaká pěkná kočka</strong></p>
</blockquote>
<blockquote>
<p>Adiós, nos vemos! <strong>Na shledanou!Tak zatím</strong></p>
</blockquote>
<blockquote>
<p>Disculpe <strong>promiňte/pardon</strong></p>
</blockquote>
<blockquote>
<p>Muchas gracias <strong>Děkuji mnohokrát!</strong></p>
</blockquote>
<blockquote>
<p>Por favor <strong>prosím</strong></p>
</blockquote>
<hr>
<h1 id="2-vocabulario">2. Vocabulario</h1>
<h3 id="por-ac%C3%A1-podr%C3%A1s-encontrar-t%C3%A9rminos-para-usar-en-el-caf%C3%A9">Por acá podrás encontrar términos para usar en el café.</h3>
<p><img src="cafe.jpg" alt="cafe"></p>
<table>
<thead>
<tr>
<th>Área</th>
<th>Español</th>
<th>Checo</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Bebidas</strong></td>
<td>Café</td>
<td>káva</td>
</tr>
<tr>
<td></td>
<td>Agua</td>
<td>voda</td>
</tr>
<tr>
<td></td>
<td>Jugo</td>
<td>džus</td>
</tr>
<tr>
<td></td>
<td>Té</td>
<td>čaj</td>
</tr>
<tr>
<td><strong>Adjetivos</strong></td>
<td>Té Caliente</td>
<td>horký    čaj</td>
</tr>
<tr>
<td></td>
<td>café Frío</td>
<td>studená káva</td>
</tr>
<tr>
<td><strong>Alimentos</strong></td>
<td>Pan</td>
<td>chléb</td>
</tr>
<tr>
<td></td>
<td>Torta</td>
<td>dort</td>
</tr>
<tr>
<td></td>
<td>Galletas</td>
<td>cookies</td>
</tr>
<tr>
<td><em>Extra</em></td>
<td>Gato</td>
<td>kočka</td>
</tr>
</tbody>
</table>
<h1 id="3-ejercicios-de-aplicaci%C3%B3n">3. Ejercicios de aplicación</h1>
<p><img src="gatos-praga.jpg" alt="gatos_praga"></p>
<p>Puedes usar este <a href="https://www.deepl.com/es/translator/l/es/cs">traductor</a> para ayudarte.</p>
<h2 id="afirmaciones">Afirmaciones</h2>
<ol>
<li>Escribe una oración para dar tu opinión sobre el café.</li>
</ol>
<p>Ej. Qué agradable el sabor de este café.</p>
<p><em>Jak příjemná je chuť této kávy</em></p>
<ol start="2">
<li>
<p>Describe al gato.</p>
</li>
<li>
<p>Da tu opinión respecto del lugar.</p>
</li>
</ol>
<p>No importa si no sabes cómo hacerlo, apóyate en el traductor y <strong>remarca las palabras que conozcas.</strong></p>
<p><em>Puedes fijarte en la estructura sintáctica de la oración y ver si se parece al español.</em></p>
<h2 id="preguntas">Preguntas</h2>
<ol>
<li>
<p>Construye una pregunta para pedir un café.</p>
</li>
<li>
<p>Pregunta dónde está el baño.</p>
</li>
<li>
<p>Pregunta si puedes acariciar al gato.</p>
</li>
</ol>
<p><s>Las soluciones están al final de la página</s></p>
<h1 id="4-links-de-inter%C3%A9s">4. Links de interés</h1>
<h3 id="por-%C3%BAltimo-te-dejo-algunos-sitios-para-que-puedas-practicar-la-pronunciaci%C3%B3n">Por último, te dejo algunos sitios para que puedas practicar la pronunciación.</h3>
<p><img src="ninos.jpg" alt="Ninos"></p>
<ul>
<li><a href="https://www.youtube.com/watch?v=XcB7mHn8N80">Aprede Checo</a></li>
<li><a href="https://www.youtube.com/watch?v=4mGGbdzisCU">LingoJump Language</a></li>
<li><a href="https://www.youtube.com/watch?v=r_EWPGIGGQg">Imperium Linguarium</a></li>
<li><a href="https://www.youtube.com/watch?v=BT1UUWG7o4g">Kosvision SM</a></li>
</ul>
<h3 id="soluciones-para-los-ejercicios-pr%C3%A1cticos">Soluciones para los ejercicios prácticos</h3>
<ol>
<li>Mohl bys mi přinést šálek kávy? <em>¿me podría traer una taza de café?</em></li>
<li>Kde jsou toalety? <em>¿Dónde está el baño?</em></li>
<li>Mohu přimět kočku milovat? <em>¿Puedo hacerle cariño al gato?</em></li>
</ol>
<hr>
<h2 id="nos-vemos-pronto-gracias-por-acompa%C3%B1arme"><em>Nos vemos pronto, gracias por acompañarme!</em></h2>
<p><img src="loconino.jpg" alt="ninoloco"></p>

</body>
</html>
