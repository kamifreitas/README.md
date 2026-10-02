# Arquivos detalhados

## index.html

É a página inicial e a porta de entrada do site. Apresenta a loja, explica como funciona o processo de compra e mostra a foto do produto em destaque, sorteada a cada carregamento pelo `script.js`. É também onde ficam os botões principais: "Ver produtos" e "Agendar visita".

## produtos.html

Contém a vitrine completa, com os botões de filtro por categoria e a barra de busca. A grade de produtos em si fica vazia no HTML (`<div id="grid-produtos">`) e é o `script.js` quem a preenche em tempo real, lendo os dados de `produtos-data.js`.

## produto.html

Página de detalhe de um único produto, aberta a partir de um link como `produto.html?id=sofa-retratil`. Assim como a vitrine, o conteúdo (`<div id="produto-detalhe">`) começa vazio e é montado pelo JavaScript conforme o `id` recebido na URL mostrando o estado da avaria, as fotos (quando houver) e os botões de contato daquele item.

## contato.html

Traz o endereço, o horário de funcionamento e o formulário de agendamento de visita. O formulário não depende de nenhum servidor: ao ser enviado, ele monta a mensagem e abre o WhatsApp já com as informações que você colocou.

## /img

Pasta reservada para as imagens do site — principalmente as fotos de avaria de cada produto, referenciadas pelo campo `avariaFotos` em `produtos-data.js`.

## css/style.css

É a parte visual do site. Usa variáveis CSS (`:root { --ink: ...; --red: ...; }`) para manter as cores consistentemente em todas as páginas, além de `flexbox` e `grid` para os layouts. A responsividade é feita com `@media`, adaptando o site para celular, tablet e computador. As animações como a faixa rolante do topo e o preview da busca todos usam `transition` e `@keyframes`.

## js/produtos-data.js

É a fonte única de dados do site: um array de objetos (`PRODUTOS`), cada um representando um produto, com nome, categoria, preço, descrição da avaria e as fotos da avaria. Qualquer produto novo, alterado ou removido é feito só neste arquivo tanto quanto a vitrine, a busca e a página de detalhe se atualizam automaticamente a partir dele.

## js/script.js

Reúne toda a lógica e as interações do site: montagem da vitrine e da página de produto, busca com preview, filtros, sorteio do produto em destaque, formulário de agendamento, faixa rolante, botão flutuante do WhatsApp e menu mobile. Cada funcionalidade é isolada em uma função própria, inicializada quando a página termina de carregar (`DOMContentLoaded`). (Futuramente sendo divididos.)

---

Acessar [Readme](README.md) · Acessar [Funcionalidades detalhadas](funcionalidades.md)
