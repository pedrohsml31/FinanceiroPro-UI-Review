# Revisão visual — Bloco 3

Bloco/versão:
Bloco 3 da v11.5 (em desenvolvimento; a versão publicada do programa é a 11.4) — NÃO é release

Commit do Financeiro Pro (repositório privado) que foi renderizado:
d20b31b05079e0e1d2bf9c74d175bd6bffee87c9

CONFIRMAÇÃO: TODOS OS DADOS DESTAS IMAGENS SÃO FICTÍCIOS. Nenhuma captura vem do banco real; nenhum nome, valor, CPF,
conta, cartão, e-mail, ID, protocolo, token ou chave é real. Ambiente gerado por `ferramentas/revisao_visual.py`.

Ambiente:
- dados sintéticos (banco montado por `ferramentas/revisao_visual.py`; titular “Usuário Exemplo da Silva”)
- sem credenciais reais (Pluggy, Gmail e IA falsas/ausentes; nada sai do PC)
- sem informações pessoais reais
- gerado em 05/10/2026; a tela é a do próprio `financeiro.py`

## 01-dashboard-ok-1280.png

Viewport:
1280x900

Tela:
Dashboard (topo)

Estado simulado:
todas as fontes cobertas; sincronização normal

Conferir:
- card “Cobertura das fontes” compacto, uma linha por instituição
- nenhuma atenção falsa (cinza = opcional, não problema)
- card de sincronização em dia
- alinhamento e margens

## 03-cobertura-expandida.png

Viewport:
1280x900

Tela:
Dashboard › Cobertura das fontes (detalhes)

Estado simulado:
todas as fontes cobertas

Conferir:
- “Última atualização” separada de “Último movimento” e de “Último documento”
- Amazon Bradesco com o nome visual correto
- Nubank VERDE mesmo sendo importação manual (aparece só como detalhe)
- Gmail cinza: ambiente isolado (não é “desconectado”)
- Banco do Brasil agrupa conta + Visa Infinite

## 02-dashboard-atencao-1280.png

Viewport:
1280x900

Tela:
Dashboard (topo)

Estado simulado:
uma fonte em atenção: fatura Amazon Bradesco esperada e não importada

Conferir:
- linha “⚠ Amazon Bradesco” em âmbar com o motivo
- as demais fontes seguem OK
- nenhum vermelho

## 04-lancamentos-1280.png

Viewport:
1280x900

Tela:
Dashboard › Lançamentos do mês

Estado simulado:
mês de referência com parcelas, avisos e fontes variadas

Conferir:
- linha = data · descrição · categoria · fonte · valor
- etiquetas só onde há decisão
- “Mercado Livre” sem produto conhecido
- Cartão Bradesco aparece como Amazon Bradesco
- filtros e botão Selecionar na barra
- nenhum dado técnico na linha

## 06-linha-normal.png

Viewport:
1280x900

Tela:
Lançamentos › linha normal

Estado simulado:
lançamento resolvido, sem etiqueta

Conferir:
- só data, descrição, categoria · fonte e valor
- sem selo, sem ícone redundante

## 07-linha-alerta.png

Viewport:
1280x900

Tela:
Lançamentos › linha com alerta útil

Estado simulado:
possível cobrança duplicada

Conferir:
- etiqueta “⚠ Possível duplicidade”
- texto do aviso só ao expandir

## 08-linha-expandida.png

Viewport:
1280x900

Tela:
Lançamentos › linha expandida

Estado simulado:
lançamento aprovado automaticamente

Conferir:
- DETALHES ÚTEIS (descrição original, data, fonte)
- POR QUE FOI CLASSIFICADO ASSIM? (confiança e evidência só aqui)
- DIAGNÓSTICO recolhido

## 09-selecao.png

Viewport:
1280x900

Tela:
Lançamentos › modo Selecionar

Estado simulado:
2 lançamentos marcados

Conferir:
- checkbox só aparece neste modo
- barra “2 selecionado(s)” com Alterar categoria / Excluir / Cancelar
- botão Selecionar destacado

## 05-lancamentos-1024.png

Viewport:
1024x800

Tela:
Dashboard › Lançamentos do mês

Estado simulado:
mesmo mês, janela estreita

Conferir:
- filtros quebram em duas linhas sem estourar
- valor e menu ⋯ continuam visíveis
- sem rolagem horizontal

## 10-configuracoes-titular.png

Viewport:
1280x900

Tela:
Configurações › Importação › Identidade do titular

Estado simulado:
titular fictício cadastrado

Conferir:
- aba Configurações destacada
- nome do titular e aliases
- monitor e pasta de entrada (caminhos sintéticos)

## 11-diagnostico-titular.png

Viewport:
1280x900

Tela:
Configurações › Diagnóstico › Testar reconhecimento do titular

Estado simulado:
linha de PIX com o nome fictício

Conferir:
- resultado “Seria IGNORADO — é transferência sua para você mesmo”
- informações técnicas com caminhos sintéticos
