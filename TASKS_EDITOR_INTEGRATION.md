# Tarefas — Integração e evolução do Editor

## Objetivo
Evoluir o editor de aplicações mantendo uma versão legada e abrindo caminho para plug-ins de bibliotecas e estilos visuais.

## Backlog sugerido
- [x] **Versionar editor atual (legado)**
  - Salvar snapshot do HTML do editor em `localStorage` usando chave de versão.
- [x] **Atalho rápido na Home**
  - Botão **Editor Rápido** para abrir o editor sem passar por todo o fluxo.
- [x] **Fluxo rápido com fallback**
  - Se não houver projeto/app, criar automaticamente um canvas inicial.
- [x] **Base para extensão por bibliotecas**
  - Estrutura de configuração para injetar `stylesheets` e `scripts` no `iframe` do editor.

## Próximas tarefas técnicas
- [ ] Adicionar seletor de versão do editor (legacy / próxima versão).
- [ ] Expor painel de configuração para adicionar/remover libs externas sem editar código.
- [ ] Definir contrato oficial de API via `postMessage` (versãoada).
- [ ] Persistir configuração de extensões por projeto.
- [ ] Criar smoke tests de abertura, load de brand kit e export PNG/SVG.

## Critérios de pronto (DoD)
- [ ] Editor abre em até 2 cliques a partir da Home.
- [ ] Versão ativa do editor registrada e auditável.
- [ ] Injeção de bibliotecas não quebra carregamento padrão.
- [ ] Exportações seguem funcionando após extensão de estilo.
