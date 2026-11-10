# TAGS E CONCEITOS DO HTML5

# Conceitos de HTML

Referência rápida das tags e atributos de HTML, organizada por tópico. Cada seção traz a finalidade de cada tag e atributo e aponta para o código completo e comentado em `fundamentos-html/`.

## Textos e formatação

Código completo: [`textos-e-formatacao/index.html`](fundamentos-html/textos-e-formatacao/index.html)

### Títulos, parágrafos e separadores

| Tag | Para que serve |
|---|---|
| `<h1>` a `<h6>` | Títulos em seis níveis hierárquicos, do mais ao menos importante |
| `<hr>` | Separador temático entre blocos de conteúdo (exibido como uma linha) |
| `<p>` | Parágrafo |
| `<br>` | Quebra de linha dentro de um texto |

### Importância, ênfase e destaque

| Tag | Para que serve |
|---|---|
| `<strong>` | Indica importância (negrito por padrão) |
| `<em>` | Indica ênfase (itálico por padrão) |
| `<b>` | Negrito visual, sem importância adicional |
| `<i>` | Itálico: termo técnico, expressão em outro idioma ou texto em outra "voz" |
| `<mark>` | Trecho destacado, como um marca-texto |
| `<small>` | Observações e textos de menor destaque, em tamanho reduzido |

### Edição, subscrito e sobrescrito

| Tag | Para que serve |
|---|---|
| `<del>` | Texto removido (exibido riscado) |
| `<ins>` | Texto adicionado (exibido sublinhado) |
| `<sub>` | Texto subscrito, abaixo da linha |
| `<sup>` | Texto sobrescrito, acima da linha |

### Abreviações e citações

| Tag | Para que serve |
|---|---|
| `<abbr>` + `title` | Abreviação; o significado aparece ao passar o mouse |
| `<q>` | Citação curta, dentro do texto (o navegador adiciona as aspas) |
| `<blockquote>` + `cite` | Citação longa, em bloco separado; `cite` indica a URL da fonte |

### Código e datas

| Tag | Para que serve |
|---|---|
| `<code>` | Trecho de código dentro de uma linha |
| `<pre>` | Texto pré-formatado: preserva espaços e quebras de linha (usado com `<code>` para blocos de código) |
| `<time>` + `datetime` | Data ou hora em formato legível por máquina |

### Menos utilizados

| Tag | Para que serve |
|---|---|
| `<wbr>` | Indica um ponto onde o navegador pode quebrar a linha, se necessário |
| `<address>` | Informações de contato da pessoa ou organização responsável pelo conteúdo |
| `<cite>` | Título de uma obra (livro, filme...) |
| `<dfn>` | Termo que está sendo definido |
| `<bdi>` | Isola um trecho cuja direção de escrita pode ser diferente do restante |
| `<bdo>` + `dir="rtl"` | Força a direção do texto (aqui, da direita para a esquerda) |
| `<s>` | Conteúdo que deixou de ser correto ou relevante (exibido riscado) |
| `<u>` | Anotação visual no texto, como uma palavra marcada (exibido sublinhado) |
| `<var>` | Variável, como em expressões matemáticas |
| `<samp>` | Saída de um programa ou terminal |
| `<kbd>` | Entrada de teclado, como um atalho |
| `<data>` + `value` | Associa um conteúdo visível a um valor legível por máquina |

---

## Links e navegação

Código completo: [`links-e-navegacao/index.html`](fundamentos-html/links-e-navegacao/index.html)

| Tag / atributo | Para que serve |
|---|---|
| `<a>` + `href` | Cria um link; `href` define o destino (link externo) |
| `target="_blank"` | Abre o link em uma nova aba |
| Link interno | Leva a outra página do mesmo projeto |
| Âncora (`#id`) | Leva ao elemento com o `id` correspondente na página |
| `mailto:` | Abre o programa de e-mail com o destinatário preenchido |
| `tel:` | Abre o aplicativo de telefone com o número indicado |
| `download` | Sugere que o navegador baixe o arquivo em vez de abri-lo |
| `<nav>` | Agrupa os links de navegação principais |
| `aria-label` | Dá um nome acessível ao elemento, descrevendo sua finalidade |
| `aria-current="page"` | Identifica qual link representa a página atual |
| `rel="noopener"` | Impede que a página aberta em nova aba controle a página original |
| `rel="noopener noreferrer"` | Além de `noopener`, impede que a página aberta saiba de onde o usuário veio |

---

## Imagens e mídias

Código completo: [`imagens-e-midias/index.html`](fundamentos-html/imagens-e-midias/index.html)

### Imagens

| Tag / atributo | Para que serve |
|---|---|
| `<img>` | Insere uma imagem |
| `src` | Caminho ou URL da imagem |
| `alt` | Texto alternativo: aparece se a imagem não carregar e é lido por leitores de tela |
| `width` e `height` | Largura e altura da imagem |
| `loading="lazy"` | A imagem só carrega quando está perto da área visível |
| `<figure>` | Agrupa um conteúdo visual (imagem, diagrama, código) |
| `<figcaption>` | Legenda do conteúdo de `<figure>` |

### Imagens responsivas

| Tag / atributo | Para que serve |
|---|---|
| `<picture>` | Permite oferecer diferentes versões da imagem (responsividade) |
| `<source>` | Define uma fonte alternativa de imagem, vídeo ou áudio |
| `media` | Condição para usar a fonte, como a largura da tela |
| `srcset` | Lista as imagens candidatas que o navegador pode escolher |
| `type` | Informa ao navegador o tipo do arquivo |

### Áudio e vídeo

| Tag / atributo | Para que serve |
|---|---|
| `<audio>` | Insere áudio (músicas, gravações). O texto dentro da tag aparece se o navegador não der suporte |
| `<video>` | Insere vídeo |
| `controls` | Exibe os controles de reprodução (pausar, volume, etc.) |
| `poster` | Imagem exibida antes de o vídeo iniciar |
| `muted` | Inicia o vídeo sem som |
| `loop` | Reinicia o vídeo sempre que ele termina |
| `<track>` | Adiciona legendas a vídeos ou áudios (arquivo `.vtt`) |
| `kind` | Tipo do texto da faixa (por exemplo, `subtitles`) |
| `srclang` | Idioma da legenda |
| `label` | Nome da legenda exibido no menu do player |

---

## Listas

Código completo: [`listas/index.html`](fundamentos-html/listas/index.html)

### Listas ordenadas e não ordenadas

| Tag / atributo | Para que serve |
|---|---|
| `<ul>` | Lista não ordenada (com marcadores) |
| `<ol>` | Lista ordenada (numerada) |
| `<li>` | Item de uma lista |
| `start` | Número em que a lista ordenada começa a contar |
| `type` | Modelo da contagem (números, letras ou algarismos romanos) |
| `value` | Define o número de um item específico |
| `reversed` | Contagem em ordem decrescente |

### Valores de `type` em listas ordenadas

| Valor | Resultado |
|---|---|
| `1` | Números (1, 2, 3) |
| `A` | Letras maiúsculas (A, B, C) |
| `a` | Letras minúsculas (a, b, c) |
| `I` | Algarismos romanos maiúsculos (I, II, III) |
| `i` | Algarismos romanos minúsculos (i, ii, iii) |

### Listas de descrição e listas aninhadas

| Tag | Para que serve |
|---|---|
| `<dl>` | Lista de termos e suas explicações |
| `<dt>` | Termo |
| `<dd>` | Explicação do termo |
| Lista aninhada | Lista dentro de um item de outra lista |

---

## Tabelas

Código completo: [`tabelas/index.html`](fundamentos-html/tabelas/index.html)

### Estrutura da tabela

| Tag / atributo | Para que serve |
|---|---|
| `<table>` | Cria a tabela |
| `<caption>` | Título da tabela |
| `<thead>` | Agrupa o cabeçalho da tabela (topo) |
| `<tbody>` | Agrupa o corpo da tabela |
| `<tfoot>` | Agrupa o rodapé da tabela |
| `<tr>` | Linha da tabela |
| `<th>` | Célula de cabeçalho (de coluna ou de linha) |
| `<td>` | Célula de dados |
| `scope` | Indica ao navegador se o cabeçalho é de coluna (`col`) ou de linha (`row`) |

### Células que ocupam mais de um espaço

| Atributo | Para que serve |
|---|---|
| `colspan` | A célula ocupa várias colunas (horizontal) |
| `rowspan` | A célula ocupa várias linhas (vertical) |

A aparência da tabela, como as bordas, é definida por CSS (`style.css`), e não por HTML.

---

## Semântica e estrutura

Código completo: [`semantica-e-estrutura/index.html`](fundamentos-html/semantica-e-estrutura/index.html)

| Tag | Para que serve |
|---|---|
| `<header>` | Cabeçalho da página ou de uma seção |
| `<nav>` | Seção de navegação (links) |
| `<main>` | Conteúdo principal da página |
| `<article>` | Conteúdo independente (artigos, notícias, publicações) |
| `<section>` | Agrupa conteúdos relacionados a um mesmo tema |
| `<aside>` | Conteúdo complementar da página |
| `<footer>` | Rodapé da página ou de uma seção |
| `<div>` | Agrupa conteúdo quando não há elemento semântico mais adequado |
| `<span>` | Agrupa um trecho dentro de uma linha, sem significado específico |
| `<search>` | Região da página que contém a funcionalidade de busca ou filtro |
| `<address>` | Informações de contato (pessoa, empresa...) |
| `&copy;` | Entidade HTML que exibe o símbolo © |

---

## Formulários

Código completo: [`formularios/index.html`](fundamentos-html/formularios/index.html)

### Estrutura e identificação

| Tag / atributo | Para que serve |
|---|---|
| `<form>` | Cria o formulário |
| `action` | Define para onde os dados são enviados |
| `method="get"` | Envia os dados pela URL (ficam visíveis) |
| `method="post"` | Envia os dados no corpo da requisição (não aparecem na URL) |
| `<fieldset>` | Agrupa campos relacionados (exibido com borda) |
| `<legend>` | Título do `<fieldset>` |
| `<label>` + `for` | Identifica um campo; `for` associa ao `id` do input |
| `<input>` | Campo onde o usuário insere um dado |
| `type` | Define o tipo do input |
| `name` | Nome do campo enviado ao servidor |
| `id` | Identifica o elemento individualmente (associado ao `label`) |

### Atributos de apoio e validação

| Atributo | Para que serve |
|---|---|
| `autocomplete` | Sugere preencher o campo com dados já usados no navegador |
| `required` | Torna o campo obrigatório |
| `placeholder` | Texto de exemplo exibido com baixa opacidade dentro do campo |
| `minlength` | Quantidade mínima de caracteres |
| `maxlength` | Quantidade máxima de caracteres |
| `min` | Valor mínimo permitido |
| `max` | Valor máximo permitido |
| `value` | Valor inicial do campo |
| `accept` | Formatos de arquivo aceitos em `type="file"` |

### Tipos de input

| Tipo | Para que serve |
|---|---|
| `text` | Texto simples |
| `email` | Endereço de e-mail |
| `password` | Senha (caracteres ocultos) |
| `number` | Número |
| `date` | Data (dia, mês e ano) |
| `time` | Horário |
| `datetime-local` | Data e horário |
| `month` | Mês e ano |
| `week` | Semana do ano |
| `color` | Seletor de cor |
| `range` | Controle deslizante |
| `file` | Seleção de arquivo |
| `tel` | Telefone |
| `url` | Endereço de site (URL) |
| `search` | Campo de pesquisa |
| `checkbox` | Caixa de marcação; permite marcar e desmarcar |
| `radio` | Opção única dentro de um grupo; os inputs do grupo compartilham o mesmo `name` |
| `hidden` | Campo oculto, enviado junto com o formulário |
| `submit` | Botão de enviar |
| `reset` | Botão de limpar o formulário |
| `button` | Botão sem ação padrão |

### Outros campos

| Tag / atributo | Para que serve |
|---|---|
| `<select>` | Lista suspensa de opções |
| `<optgroup>` | Separa as opções do `<select>` em grupos |
| `<option>` | Opção dentro do `<select>` ou do `<datalist>` |
| `<datalist>` | Lista de sugestões que permite ao usuário digitar; é ligada ao input pelo atributo `list` |
| `list` | Indica o `id` do `<datalist>` associado ao input |
| `<textarea>` | Área para texto de várias linhas |
| `cols` e `rows` | Largura e altura da área de texto |

---

## Metadados e SEO

Código completo: [`metadados-e-seo/index.html`](fundamentos-html/metadados-e-seo/index.html)

| Tag / atributo | Para que serve |
|---|---|
| `lang` | Idioma do conteúdo da página |
| `<head>` | Informações sobre a página (título, metadados, ícone e links de recursos) |
| `<meta charset>` | Codificação de caracteres, para exibir corretamente acentos como ã, ç e é |
| `<meta name="viewport">` | Controla como a página se ajusta à área visível do dispositivo |
| `width=device-width` | A largura da página acompanha a largura do dispositivo |
| `initial-scale=1.0` | Define a escala inicial em 100% |
| `<title>` | Título da página, exibido na aba do navegador |
| `<meta name="description">` | Descrição resumida do assunto da página |
| `<meta name="author">` | Informa quem criou a página |
| `<link rel="stylesheet">` | Relaciona o documento a um arquivo CSS externo |
| `<script src>` | Conecta um arquivo JavaScript externo à página |
| `<link rel="icon">` | Ícone da página (favicon), exibido na aba do navegador |
| `<meta name="theme-color">` | Cor de tema usada pelo navegador em contextos compatíveis |

---

## Acessibilidade

Código completo: [`acessibilidade/index.html`](fundamentos-html/acessibilidade/index.html)

| Recurso | Para que serve |
|---|---|
| Link de salto | Permite pular direto ao conteúdo principal: o `href="#id"` leva ao elemento com esse `id` |
| `<main id>` | Conteúdo principal, com `id` para receber o link de salto |
| `<button>` + `aria-label` | Botão que só tem símbolo (como ×) recebe um nome acessível para leitores de tela |
| `alt` | Descreve a imagem para quem não a vê |
| `<label>` + `for` | Associa o rótulo ao campo, para leitores de tela e para ampliar a área de clique |

Veja também: `aria-label` e `aria-current` em [Links e navegação](#links-e-navegação).

---

## Recursos avançados

Código completo: [`recursos-avancados/index.html`](fundamentos-html/recursos-avancados/index.html)

| Tag / atributo | Para que serve |
|---|---|
| `<details>` | Área que o usuário pode expandir ou recolher |
| `<summary>` | Título clicável que abre e fecha o `<details>`; o conteúdo fica abaixo dele |
| `<dialog>` | Caixa de diálogo |
| `open` | Faz a caixa de diálogo (ou o `<details>`) aparecer aberta |
| `<form method="dialog">` | Formulário dentro do `<dialog>` cujo botão fecha a caixa |
| `<template>` | Guarda um modelo de HTML que não é exibido diretamente; é usado depois, com JavaScript |
| `<iframe>` | Incorpora outra página ou documento dentro da página atual |
| `<canvas>` | Área de desenho controlada por JavaScript; o texto dentro aparece se não houver suporte |
| `<svg>` | Gráfico vetorial que pode ser desenhado direto no HTML |
| `<circle>` | Círculo dentro do SVG: `cx` e `cy` definem o centro, `r` o raio e `fill` a cor |

---

## Fontes de referência

- [MDN Web Docs: elementos HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element)
- [WHATWG HTML Living Standard](https://html.spec.whatwg.org/)
