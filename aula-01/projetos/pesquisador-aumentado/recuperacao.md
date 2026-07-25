[← Book do Funil](./index.html)

# Recuperação de Checkout: Pesquisador Aumentado™
## Sequência de re-elevação de consciência (setup pré-lançamento)

**Skill:** `/recuperacao-funil`
**Data:** 25 de julho de 2026
**Fonte:** `KB-recuperacao.md` (método e verbatim) + `offerbook.md` (oferta/ticket) + `copy.md` (Big Idea, mecanismos, bullets) + `emails/trilhas.md` (trilha de nutrição já existente)
**Status:** Checkout existe no Hotmart, mas o rastreio de comportamento (cartão recusado, boleto, carrinho abandonado) ainda não foi confirmado. Este documento entrega o **SETUP**: a cascata pronta pra ativar assim que cada rastreio existir, não uma sequência já disparando.

---

## Gate: o que está confirmado e o que falta

Você confirmou:
- **Checkout:** já existe no Hotmart.
- **Comportamentos rastreados hoje:** nenhum confirmado ainda ("não sei").
- **Downsell:** não existe ainda.
- **Canais:** não confirmados (assumindo e-mail como canal mínimo, já que a trilha de `/email-funil` está pronta na mesma ferramenta).

Por isso, a cascata abaixo é **plano pronto pra ativar**, degrau por degrau, conforme cada rastreio for confirmado no Hotmart. Isso está registrado em `pendencias.md` (itens 7, 8 e 9).

---

## O que cada degrau da cascata exige do Hotmart

| Degrau | Rastreio necessário | Normalmente | Ação antes de ativar |
|---|---|---|---|
| Cartão recusado | Hotmart sinalizar falha de pagamento por cartão | **Nativo** do gateway | Confirmar no painel Hotmart se há webhook/notificação de "compra recusada" habilitado |
| Boleto gerado | Hotmart sinalizar emissão de boleto + data de vencimento | **Nativo** do gateway | Confirmar notificação de "boleto gerado" habilitada |
| Carrinho abandonado | Captura de e-mail/contato antes do pagamento + integração com automação | **Exige integração** | Confirmar se o plano Hotmart tem recuperação de carrinho nativa, ou conectar a uma automação externa (a mesma ferramenta de disparo da trilha de e-mails) |
| Downsell | Nenhum rastreio extra, mas exige o produto existir | Depende de decisão do dono | Definir o produto de downsell (pendência 8) |
| Re-nutrição (nível 4) | Nenhum rastreio extra, reaproveita a trilha de e-mails já pronta | Já existe | Nenhuma ação técnica; só decidir o ponto de reentrada na trilha |

---

## A cascata (do mais quente ao mais frio)

```
1. Cartão recusado      → quentíssimo, tentou pagar
2. Boleto gerado         → muito quente, escolheu pagar
3. Carrinho abandonado   → quente, mas com objeção
4. Downsell              → esfriando, barreira de preço
5. Re-nutrição (nível 4) → frio, reconstruir o caminho
```

Cada degrau só dispara se o anterior não converteu. A leitura vem do KB: quem tentou pagar (cartão recusado) está mais quente que quem só chegou ao carrinho.

---

## 1. Cartão recusado

**Leitura:** tentou pagar, a intenção já foi provada. É o degrau mais quente da cascata.
**Abordagem:** tom direto, oferece trocar o meio de pagamento; desconto é opcional, sem percentual definido na fonte.
**Cadência sugerida:** mensagem 1 imediata (poucos minutos após a falha), mensagem 2 em 24h se não resolver.

### Mensagem 1 — Imediata

**Assunto:** Seu pagamento não passou, mas seu acesso está reservado

Prof. {{primeiro_nome}},

Seu pagamento do Pesquisador Aumentado™ não foi aprovado. Acontece por vários motivos, geralmente é rápido de resolver.

Duas opções:
- Tentar de novo com outro cartão
- Pagar por boleto ou Pix

O acesso ao método continua reservado pra você. O link é o mesmo:

https://pay.hotmart.com/O106631740D

Prof. Dr. Sergio Rolemberg Farias

**CTA:** "Concluir minha compra" → https://pay.hotmart.com/O106631740D

### Mensagem 2 — 24h depois (se não resolveu)

**Assunto:** Ainda dá tempo de resolver o pagamento

{{primeiro_nome}},

Seu acesso ao Pesquisador Aumentado™ continua reservado, mas notei que o pagamento de ontem não foi concluído.

Se foi problema com o cartão, o boleto ou o Pix resolvem na hora. [DONO: decidir se oferece desconto neste degrau, e qual percentual, a fonte não crava valor].

https://pay.hotmart.com/O106631740D

Prof. Dr. Sergio Rolemberg Farias

---

## 2. Boleto gerado

**Leitura:** escolheu pagar, mas ainda não pagou. Interesse maior que carrinho abandonado.
**Abordagem:** empurrar para o cartão (mais rápido que esperar o boleto compensar), com desconto opcional.
**Cadência sugerida:** 1 dia antes do vencimento do boleto.

### Mensagem — 1 dia antes do vencimento

**Assunto:** Seu boleto vence amanhã, prefere já ter acesso hoje?

{{primeiro_nome}},

O boleto do Pesquisador Aumentado™ vence amanhã. Se preferir não esperar a compensação, o cartão libera o acesso na hora.

https://pay.hotmart.com/O106631740D

Prof. Dr. Sergio Rolemberg Farias

**CTA:** "Pagar com cartão e liberar agora" → https://pay.hotmart.com/O106631740D

---

## 3. Carrinho abandonado

**Leitura:** chegou ao checkout, não chegou a tentar pagar. Está com objeção, algo travou a decisão.
**Abordagem:** mensagem leve, tom de "aconteceu algo errado?", nunca pressão.
**Cadência:** 30 minutos depois (janela explícita na fonte).

### Mensagem — 30 minutos depois

**Assunto:** Alguma dúvida antes de continuar?

{{primeiro_nome}},

Vi que você chegou até a página do Pesquisador Aumentado™ e não finalizou.

Se ficou alguma dúvida, sobre o método, sobre a garantia de 7 dias, ou sobre como funciona na prática, é só responder este e-mail. Eu leio e respondo pessoalmente.

Se preferir voltar direto, o link é este:

https://pay.hotmart.com/O106631740D

Prof. Dr. Sergio Rolemberg Farias

---

## 4. Downsell

**Leitura:** não converteu em nenhuma das três abordagens diretas. Barreira de preço, não de crença.
**Abordagem:** oferecer um produto mais barato que o e-book completo (R$127).
**Status:** **[PRODUTO DE DOWNSELL A DEFINIR PELO DONO DA OFERTA]**. Não existe ainda. Recomendação (não decisão): um recorte do e-book, por exemplo só o Capítulo 5 (o roteiro pronto de perguntas por fase do TCC) ou a isca digital "7 Perguntas Socráticas" com um pequeno complemento pago, a um ticket bem abaixo de R$127.

### Mensagem — modelo (aguarda produto definido)

**Assunto:** Uma versão mais enxuta do método, se o momento não é agora

{{primeiro_nome}},

Talvez R$127 não seja o momento certo agora. Entendo.

Separei uma versão mais enxuta: **[NOME DO PRODUTO DE DOWNSELL]**, por **[PREÇO DO DOWNSELL]**. [DESCRIÇÃO CURTA DO QUE ENTREGA].

[LINK DO CHECKOUT DO DOWNSELL]

Prof. Dr. Sergio Rolemberg Farias

---

## 5. Re-nutrição (re-elevação para o nível de consciência do problema)

**Leitura:** não converteu nem no downsell. Esfriou, precisa reconstruir o caminho.
**Abordagem:** joga o lead de volta para a consciência da dor (ciclo corretivo, Corretor Compulsivo), não tenta vender de novo direto.
**Como:** reaproveita a trilha de nutrição já pronta em `emails/trilhas.md`, reentrando a partir do **E2** ("O problema não é o aluno que some"), não do E1 (que já foi consumido com a isca). Reinicia a partir da dor estrutural, sem repetir a entrega da isca.

**Sequência de reentrada:** E2 → E3 → E4 → E5 → E6 → E7 → (nova tentativa de) E8-E10, com um espaçamento maior entre os envios (sugestão: dobrar os intervalos originais, já que esse lead já viu o pitch uma vez).

---

## Mapa de disparos (canal + momento)

| Degrau | Canal | Momento |
|---|---|---|
| Cartão recusado (msg 1) | E-mail | Imediato após a falha |
| Cartão recusado (msg 2) | E-mail | 24h depois, se não resolvido |
| Boleto gerado | E-mail | 1 dia antes do vencimento |
| Carrinho abandonado | E-mail | 30 minutos depois |
| Downsell | E-mail | 48h após a última tentativa de recuperação direta |
| Re-nutrição | E-mail (trilha existente) | Reentrada a partir do E2, espaçamento dobrado |

WhatsApp e SMS não estão confirmados como canais disponíveis (pendência 9). Se existirem, os mesmos textos podem ser adaptados para mensagem curta.

---

## Regras aplicadas

- Nenhuma mensagem usa desconto/percentual inventado: onde a fonte não crava valor, ficou marcado como decisão do dono.
- Nenhuma prova nova foi inventada; as mensagens de recuperação não citam depoimento algum.
- Sem travessão em nenhuma copy aplicada.
- Nenhum disparo real acontece sem sua aprovação.

---

## Próximos passos

1. Confirmar no painel Hotmart quais notificações de comportamento (cartão recusado, boleto, carrinho) estão ativas.
2. Decidir o produto de downsell.
3. Confirmar canais disponíveis além de e-mail.
4. Só depois, conectar esta cascata a uma automação real de disparo.

---

*Recuperação gerada por `/recuperacao-funil`, lendo `KB-recuperacao.md` + `offerbook.md` + `copy.md` + `emails/trilhas.md`.*
