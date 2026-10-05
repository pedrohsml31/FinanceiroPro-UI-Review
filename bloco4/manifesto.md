# Revisão visual — Bloco 4

Bloco/versão:
Bloco 4 da v11.5 (em desenvolvimento; a versão publicada do programa é a 11.4) — NÃO é release

Commit do Financeiro Pro (repositório privado) que foi renderizado:
72a6d719be81f493cdf1ab155b5296c4816e7e70

CONFIRMAÇÃO: TODOS OS DADOS DESTAS IMAGENS SÃO FICTÍCIOS. Nenhuma captura vem do banco real; nenhum nome, valor, CPF,
conta, cartão, e-mail, ID, protocolo, token ou chave é real. Ambiente gerado por `ferramentas/revisao_visual.py`.

PDF de revisão:
review.pdf

Finalidade:
arquivo navegável (1 página por captura, na ordem abaixo) destinado à inspeção visual pelo ChatGPT, porque o conector do
GitHub entrega PNG como binário/base64. O PDF contém EXCLUSIVAMENTE as mesmas 5 capturas sintéticas listadas aqui (conferido pixel a
pixel e por SHA-256 antes de publicar); nenhuma tela nova e nenhum dado real.

Ambiente:
- dados sintéticos (banco montado por `ferramentas/revisao_visual.py`; titular “Usuário Exemplo da Silva”)
- sem credenciais reais (Pluggy, Gmail e IA falsas/ausentes; nada sai do PC)
- sem informações pessoais reais
- gerado em 05/10/2026; a tela é a do próprio `financeiro.py`

## 01-auxilio-saude-visao-principal-1280.png

Viewport:
1280x900

Tela:
Benefícios › Auxílio-Saúde (visão principal)

Estado simulado:
despesas a solicitar, um pedido solicitado e um aprovado

Conferir:
- 4 totais: A solicitar / Solicitado / Aprovado / Pago, sem protocolo nem ID no topo
- botões Ver despesas e Pedidos feitos
- início da lista “A solicitar”
- “Ferramentas e detalhes” recolhido mais abaixo

## 02-a-solicitar-competencia-1280.png

Viewport:
1280x900

Tela:
Auxílio-Saúde › A solicitar

Estado simulado:
competência confirmada, provável (provisória) e a confirmar

Conferir:
- cada linha: descrição, valor ELEGÍVEL (270,00 de 277,09 no plano), competência e estado dela
- ✓ confirmada com a data do pagamento
- ◌ provável com “Pagamento da fatura ainda não confirmado”
- ⚠ a confirmar, sem inventar o mês
- “possíveis” recolhido

## 03-ja-solicitei-modal-1280.png

Viewport:
1280x900

Tela:
Auxílio-Saúde › modal “Já solicitei”

Estado simulado:
2 despesas marcadas

Conferir:
- despesas incluídas e valor elegível total
- campos: data do pedido, número/protocolo, situação inicial, observação
- “Mais detalhes” recolhido
- texto deixando claro que o Financeiro não envia nada ao portal

## 04-pedido-existente-expandido-1280.png

Viewport:
1280x900

Tela:
Auxílio-Saúde › Pedidos já feitos (um expandido)

Estado simulado:
AS-001 solicitado (competência registrada diferente da calculada) e AS-002 aprovado

Conferir:
- lista compacta: data, nº de despesas, valor e status agrupado
- expandido: protocolo, status na plataforma, aprovado/pago, despesas e competência de cada uma
- aviso discreto “competência histórica possivelmente inconsistente — nenhum pedido foi alterado”

## 05-auxilio-saude-1024.png

Viewport:
1024x800

Tela:
Benefícios › Auxílio-Saúde

Estado simulado:
mesma tela em janela estreita

Conferir:
- os 4 totais não quebram nem estouram
- linhas legíveis, valor visível
- sem rolagem horizontal
