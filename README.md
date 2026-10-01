# Saldão Total

## 1. Introdução / Apresentação do problema

### 1.1 Descrição

O Saldão Total é um site desenvolvido para uma loja de móveis e eletrodomésticos que comercializa produtos com algum tipo de avaria (riscos, amassados, embalagem violada, entre outros). O objetivo do projeto é apresentar a loja, o catálogo de produtos e as principais informações de contato de um jeito simples, organizado e fácil de acessar, permitindo que o cliente conheça o que está disponível, veja o estado de cada avaria e o preço, e agende uma visita à loja diretamente pelo WhatsApp.

A loja não realiza entregas: o modelo de negócio é baseado em consultas e visitas agendadas, já que o cliente precisa conferir o produto e a avaria pessoalmente antes da compra.

### 1.2 Problema a ser resolvido

Antes do site, a loja tinha dificuldade em divulgar seus produtos e informações de forma organizada para os clientes. Não era fácil para as pessoas saberem o que havia disponível no momento, qual o estado de cada item ou como agendar uma visita. O site resolve esse problema ao reunir, em um só lugar:

- a vitrine completa de produtos, com busca e filtro por categoria;
- a condição detalhada da avaria e o preço de cada item, numa página própria;
- um canal direto de agendamento com a loja pelo WhatsApp, sem depender de ligação.

Assim, o cliente consegue explorar o catálogo, conferir os detalhes de cada produto e marcar uma visita antes mesmo de sair de casa.

## 2. Metodologia / Perspectiva de solução

### 2.1 Requisitos operacionais

- Pode ser acessado de qualquer computador, notebook, tablet ou celular;
- Funciona em qualquer navegador de internet atualizado, com conexão à rede;
- Não exige instalação de nenhum programa ou aplicativo adicional;
- O agendamento e o contato com a loja acontecem pelo WhatsApp — não há entrega, apenas visita presencial agendada.

### 2.2 Ferramentas utilizadas

- HTML5 - estrutura das páginas;
- CSS3 - estilização visual (cores, layout, responsividade);
- JavaScript - interações do site, como busca, filtros e geração dinâmica dos produtos;
- Visual Studio Code - ambiente de desenvolvimento;
- Git / GitHub - controle de versão e armazenamento do código;
- GitHub Pages - hospedagem do site.

### 2.3 Funcionalidades

- Apresentação da loja na página inicial, com produto em destaque sorteado a cada visita;
- Vitrine completa de produtos, com filtro por categoria (móveis / eletrodomésticos);
- Busca por produto no cabeçalho, disponível em todas as páginas, com preview dos resultados enquanto o cliente digita e redirecionamento para a vitrine filtrada;
- Página individual para cada produto, mostrando o estado da avaria, fotos da avaria (quando cadastradas) e o preço;
- Botão de WhatsApp em cada produto, já com uma mensagem pronta perguntando sobre aquele item específico;
- Formulário de agendamento de visita (nome, telefone, data e horário) que monta a mensagem e abre o WhatsApp automaticamente;
- Botão flutuante de WhatsApp presente em todas as páginas;
- Interface responsiva, adaptada para computador e celular.

### 2.4 Estrutura de arquivos e pastas

```
saldao-total/
│   index.html        - página inicial
│   produtos.html     - vitrine de produtos
│   produto.html      - página de detalhe de um produto específico
│   contato.html      - contato e agendamento
│   README.md
│
├───css
│       style.css
│
├───img
│
└───js
        produtos-data.js  - dados dos produtos (fonte única usada pelas páginas)
        script.js         - funcionalidades e interações do site
```

## Autores

Gabriel Luiz Petry, Gabrielly Baungartner, Kamilly Freitas e Rafael Gomes.
