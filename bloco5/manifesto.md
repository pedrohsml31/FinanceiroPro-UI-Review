# Revisão visual — Bloco 5

Bloco/versão:
Bloco 5 da v11.5 (em desenvolvimento; a versão publicada do programa é a 11.4) — NÃO é release

Commit do Financeiro Pro (repositório privado) que foi renderizado:
1f4f6f2e57bdf693265ff5ee16879f5a561de2bf

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
- gerado em 06/10/2026; a tela é a do próprio `financeiro.py`

## 01-revisao-1280.png

Viewport:
1280x900

Tela:
Revisão (caixa de decisões)

Estado simulado:
12 decisões (23 lançamentos); 2 novas; abas Novas/Todas, busca e filtros

Conferir:
- cabeçalho “Revisão — Decisões que precisam de você” com “2 novas · 10 anteriores”
- 1 cartão = 1 decisão; as NOVAS (faixa âmbar) vêm primeiro
- cada cartão: o que é, quanto, de onde e quando, e a PERGUNTA
- sugestão forte × palpite em linguagem humana (sem “confiança = 0,93”)
- ações principais visíveis; nenhum ID, fingerprint, MCC ou descrição bruta

## 02-grupo-expandido-1280.png

Viewport:
1280x900

Tela:
Revisão › cartão de GRUPO expandido

Estado simulado:
3 lançamentos da mesma academia = 1 decisão

Conferir:
- “A decisão vale para os 3 lançamentos juntos (R$ …)”
- o botão diz o alcance: “Confirmar Saúde nos 3 lançamentos”
- lista das 3 linhas (data, nome, valor)
- link “Revisar linha a linha no modo técnico”

## 03-sugestao-por-que-1280.png

Viewport:
1280x900

Tela:
Revisão › sugestão com “Por quê?” aberto

Estado simulado:
sugestão forte do histórico, explicada

Conferir:
- botão único “Confirmar Alimentação” (1 clique)
- “O que eu vi” em português; “Por que estou perguntando” separado
- “Detalhes técnicos” recolhido (confiança, fp, IDs ficam lá)

## 04-sem-sugestao-1280.png

Viewport:
1280x900

Tela:
Revisão › possível cobrança repetida (decisão própria, nunca dentro de um grupo)

Estado simulado:
um débito com outro igual em 25/03

Conferir:
- a pergunta é só “este lançamento é um duplicado?”
- mostra “Este lançamento” e o “Possível correspondente” (valor e data)
- botões “Não é duplicado — …” e “É duplicado — não registrar”
- “Por quê?”: o outro débito igual; nenhuma decisão automática
- (a categoria só aparece depois de dizer que NÃO é duplicado)

## 05-revisao-1024.png

Viewport:
1024x800

Tela:
Revisão (caixa de decisões)

Estado simulado:
mesma tela em janela estreita

Conferir:
- os botões do cartão quebram em outra linha, sem estourar
- valor e título legíveis
- sem rolagem horizontal
