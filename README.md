# Agenda Febracis

Visualizador da agenda Google Calendar com filtros por unidade (BEL/VIX/THE), treinamento e período. Botão de copiar lista pra WhatsApp.

## Acessar online

https://agentecomercial.github.io/agenda-febracis/agenda.html

Na primeira visita, a tela pede o **Client ID OAuth** — siga os passos exibidos pra criar no Google Cloud Console (uma vez só).

## Funcionalidades

- Login Google OAuth (escopo `calendar.readonly`)
- Filtros: unidade (BEL/VIX/THE), passado/futuro com várias janelas, treinamento (dinâmico), busca livre
- Stats clicáveis com toggle (drilldown por unidade)
- Copiar lista filtrada em formato WhatsApp
- Copiar evento individual

## Rodar localmente (Windows, sem instalar nada)

Duplo-clique em `serve-agenda.ps1` (ou clique direito → "Executar com PowerShell"). Sobe um servidor local na porta 5500 e abre o navegador.

## Configuração OAuth no Google Cloud

Necessário criar um **Client ID OAuth** (tipo Aplicativo da Web) com a Calendar API habilitada. Em "Origens JavaScript autorizadas":

- `http://localhost:5500` e `http://127.0.0.1:5500` (desenvolvimento local)
- `https://agentecomercial.github.io` (produção GitHub Pages)

## Códigos de unidade

| Código | Cidade |
|---|---|
| BEL | Belém |
| VIX | Vitória |
| THE | Teresina |
