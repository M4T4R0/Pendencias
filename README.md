# Pendências

Controle das pendências de desenvolvimento de produtos de móveis. Para cada produto, acompanha as etapas 3D, 2D, VOL, CAD, MAN, CUSTO e EAN, e guarda as tarefas soltas com prazo. Funciona offline e cabe num pendrive.

## O que faz
- Organiza os produtos por linha e mostra, para cada etapa, se está OK, em andamento (…), em revisão (REV) ou não se aplica (—).
- Guarda pendências com prazo e prioridade, ligadas a um produto ou a uma linha.
- Avisa o que está atrasado, o que vence hoje, os produtos parados há dias, as etapas puladas e os códigos repetidos.
- Tem comandos rápidos, como `DM0800 vol ok` (marca a etapa) e `#everest ajustar ranhura` (cria uma pendência ligada à linha).
- Importa uma lista de produtos colada do Excel, e exporta ou importa backup em JSON.

## Como abrir
Abra `app/pendencias.html` no Microsoft Edge ou no Google Chrome. Não precisa instalar nada nem de internet.

- Na primeira vez, o app abre com os dados de exemplo (a lista de produtos embutida).
- Em **? Ajuda**, escolha a pasta onde o app grava o `pendencias.json`. Ele grava também uma cópia por dia em `backup\`.
- Para começar com os seus dados, use **? Ajuda > Importar backup**. O arquivo [exemplos/pendencias.exemplo.json](exemplos/pendencias.exemplo.json) mostra o formato.

A versão de pendrive (`Pendencias.exe`, com ícone no relógio e notificações do Windows) usa este mesmo `pendencias.html`. O código-fonte desse executável não faz parte deste repositório; o [LEIA-ME.txt](LEIA-ME.txt) explica como usar essa versão.

## Como usar
1. **Cadastro**: crie as linhas e os produtos, ou cole a lista do Excel (código e descrição).
2. **Etapas**: clique na etapa do produto para mudar o estado, ou use os comandos rápidos.
3. **Pendências**: anote o que falta, com prazo. Atrasadas e as de hoje aparecem em destaque.
4. **Avisos do cadastro**: confira os produtos parados e os itens a rever.
