# AGENTS.md

## Visão geral

Esse site é feito pensando nos fãs de Berserk que querem algum lugar para saber notícias, informações ou querem apenas conversar sobre o mangá de Kentaro Miura.

## Tecnologias

 HTML, CSS e JavaScript (Vanilla JS)
 Node.js com Express para o servidor
 MySQL hospedado em uma Máquina Virtual (VM) Linux
 Chart.js para exibição dos gráficos do Dashboard

## Comandos

 Estruturas do código: while, if, else, else if, for, and (&&), or (||), strings 
 Elementos HTML/DOM: input, label, div, button, alert

## Arquitetura

- Pasta public/: Páginas do site (index.html, login.html, cadastro.html, dashboard.html), arquivos .css e scripts .js que rodam no navegador
- Pasta src/: Código do servidor dividido em routes/ (rotas), controllers/ (regras), models/ (consultas SQL) e config/ (conexão com o banco)
- Fluxo da requisição O JS do navegador faz um fetch(), a rota recebe e chama o controller, o controller usa o model para buscar no MySQL e devolve a resposta em JSON para a tela.
- Onde criar arquivos Páginas e estilos em public/, novas rotas e regras de banco dentro de src/.

## Padrões de desenvolvimento

- Utilizar const por padrão e let apenas quando houver necessidade de reatribuição (ex: em laços for e contadores).
- Nomenclatura em camelCase para variáveis e funções (ex: validarCadastro, idUsuario).

## Cuidados e restrições

- Não alterar nada que já esteja no código, apenas adicionar informações. Qualquer mudança que seja feita precisa ser documentada e explicar onde foi feita e porque ela foi feita, explicando sempre a necessidade dela.
- Anotar todas as ajudas de IA no Diário de Prompts obrigatório.

## Regra geral: 

Antes de implementar uma alteração, siga as tecnologias, arquitetura, convenções e restrições descritas neste documento. Caso alguma informação esteja ausente, analise o código existente e siga os padrões já adotados no projeto.