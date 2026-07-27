[← Book do Funil](./index.html)

# Pendências — Pesquisador Aumentado™

Registro único de decisões do dono da oferta, agrupadas por decisão (uma decisão pode afetar vários arquivos). Atualizado com a página de captura da isca publicada no ar (27 de julho de 2026).

**Placar:** 6 aplicadas · 0 parciais · 4 abertas

---

## 1. Bônus de lançamento pago

- [x] **Status:** Aplicada (25/07/2026)
- **Decisão:** acesso antecipado com desconto ao próximo produto do dono da oferta, "Publicar ou Perecer" (substitui a recomendação original do offerbook, "acesso a grupo de professores").
- **Onde foi aplicado:** `offerbook.md` (BLOCO 2, BLOCO 5, LP Versão A, Lacunas) + `offerbook.html` · `copy.md` (regra de honestidade, Fase 2) + `copy.html` · `emails/trilha-lancamento-email-8.html` e `emails/trilhas.md`/`.html` (E8, lançamento).

## 2. Depoimento direto de professor

- [ ] **Status:** Aberto
- **O quê decidir:** hoje só existe o depoimento do Pedro (aluno, UFCG), rotulado como prova de mecanismo. Falta um depoimento de um professor que aplicou o método.
- **Onde aparece:** `offerbook.md` (Lacunas), `copy.md` (arquitetura de prova), `emails/trilha-lancamento-email-6.html` e `emails/trilhas.md`/`.html` (E6, marcado `[SEM PROVA AINDA]`).
- **Como resolver:** cole aqui o depoimento (nome, curso/universidade, uma citação) quando tiver um professor que testou o método. Até lá, o placeholder permanece.

## 3. Link da isca digital (página de captura)

- [x] **Status:** Aplicada (27/07/2026)
- **O que foi feito:** conteúdo escrito (`isca-7-perguntas-socraticas.md`/`.html`, a partir dos 4 tipos de pergunta do Capítulo 2), PDF gerado via `weasyprint` (`isca-7-perguntas-socraticas.pdf`, 1 página), e uma página de captura nova (`isca/index.html`, formulário nome+e-mail) publicada dentro do repositório real `48cork/pesquisador-aumentado-landing`, no mesmo sistema visual do `index.html` do site.
- **URLs no ar:**
  - Página de captura: `https://48cork.github.io/pesquisador-aumentado-landing/isca/`
  - PDF direto: `https://48cork.github.io/pesquisador-aumentado-landing/isca/As-7-Perguntas-Socraticas-Pesquisador-Aumentado.pdf`
- **Onde foi aplicado:** `emails/trilha-lancamento-email-1.html` e `emails/trilhas.md`/`.html` (E1, CTA aponta direto pro PDF, já que quem recebe o E1 já deu o e-mail antes).
- **Nota:** a captura da página `isca/` ainda não tem CRM/webhook real conectado (placeholder `[PLUG: WEBHOOK_CRM]` comentado no código, mesmo padrão já usado no `quiz/` do site). O formulário funciona (revela o botão de download), mas o lead não é salvo em lugar nenhum ainda.
- **O quê ainda falta decidir:** a página de captura (formulário de e-mail) e o link de entrega ainda não existem.
- **Onde aparece:** `emails/trilha-lancamento-email-1.html` e `emails/trilhas.md`/`.html` (E1, placeholder `[LINK DA ISCA DIGITAL]`).
- **Como resolver:** gere o PDF do `isca-7-perguntas-socraticas.html`, suba numa página de captura, e cole aqui a URL final.

## 4. Link do checkout

- [x] **Status:** Aplicada (25/07/2026)
- **Valor aplicado:** `https://pay.hotmart.com/O106631740D`
- **Onde foi aplicado:** `emails/trilha-lancamento-email-8.html`, `-9.html`, `-10.html`, `emails/trilhas.md`/`.html`, `recuperacao.md`/`.html` (todas as ocorrências de `[LINK DO CHECKOUT]`, exceto `[LINK DO CHECKOUT DO DOWNSELL]` em `recuperacao.md`, que continua pendente da decisão 8).

## 5. Link de descadastro (compliance)

- [ ] **Status:** Aberto
- **O quê decidir:** o rodapé de todos os 10 e-mails tem um placeholder `[LINK DE DESCADASTRO]`, exigido pela sua ferramenta de disparo (ex.: link de unsubscribe automático do Mailchimp, ActiveCampaign, etc.).
- **Onde aparece:** rodapé de `emails/trilha-lancamento-email-1.html` até `-10.html`.
- **Como resolver:** normalmente sua ferramenta de disparo injeta esse link automaticamente (tag tipo `*|UNSUB|*`); confirme a sintaxe da sua ferramenta e eu troco em todos os 10 de uma vez.

## 6. Escolha final da headline (identidade vs. contraste B2C)

- [x] **Status:** Aplicada (25/07/2026)
- **Decisão:** headline de identidade, substituindo D2 (contraste B2C) como #1.
  > "Você passou anos aprendendo a fazer perguntas certas. Agora existe um método para ensinar seus alunos a fazê-las, antes de chegar na sua sala."
- **Onde foi aplicado:** `offerbook.md` + `offerbook.html` (regenerado por completo a partir do `.md`, aplicando os tokens do `DESIGN.md`; a versão anterior do `.html` usava um tema genérico verde/serifado, não a identidade da marca) e `copy.md` (nova seção "Headline final escolhida pelo dono", Checkpoint e Resumo atualizados). D2 permanece registrada como variante testável em ambos os arquivos.

## 7. Rastreio de comportamento no Hotmart (cartão recusado, boleto, carrinho)

- [x] **Status:** Aplicada — confirmado direto no painel Hotmart (25/07/2026)
- **O que foi confirmado:**
  - **Carrinho abandonado:** automação nativa via WhatsApp já ativa (`Whatsapp_8075552`), disparando a mensagem padrão da Hotmart. Pré-requisito "solicitação de telefone no checkout" confirmado ativo.
  - **Cartão recusado por saldo insuficiente:** recuperação automática via Pix + Cartão de Crédito já ativa nativamente.
  - **Chat de WhatsApp para suporte de pagamentos recusados:** ativado agora, com mensagem customizada ("Seu pagamento não foi aprovado, mas seu acesso ao Pesquisador Aumentado™ está reservado. Fale comigo aqui que resolvemos rápido.") e número **+55 83 99118-3123 (PROVISÓRIO, ver item 10)**.
  - **Boleto:** vence em 2 dias úteis, disponível de segunda a sexta.
- **Onde aparece:** `recuperacao.md`/`.html` (a cascata sai do modo "setup"; degraus de cartão recusado e carrinho abandonado agora rodam nativamente pelo Hotmart, não só por e-mail).
- **Ação:** nenhuma resposta pendente. `recuperacao.md`/`.html` precisa ser regerado pra refletir o rastreio real (fora do escopo desta atualização; avise quando quiser rodar).

## 8. Produto de downsell

- [ ] **Status:** Aberto
- **O quê decidir:** não existe produto de downsell (oferta mais barata pra quem não fecha no R$127). Recomendação registrada em `recuperacao.md`: recorte do e-book (ex.: só o Capítulo 5) ou a isca com complemento pago.
- **Onde aparece:** `recuperacao.md`/`.html` (degrau 4 da cascata, mensagem com placeholders `[NOME DO PRODUTO]`, `[PREÇO]`, `[DESCRIÇÃO]`).
- **Como resolver:** decida o produto e o preço, ou responda "usar a recomendação".

## 9. Canais de recuperação além de e-mail

- [x] **Status:** Aplicada — WhatsApp confirmado (25/07/2026)
- **O que foi confirmado:** WhatsApp já está em uso nativamente no Hotmart, por dois caminhos: a automação de carrinho abandonado (`Whatsapp_8075552`) e o chat de suporte de pagamento recusado (número provisório, ver item 10). SMS não foi mencionado, considerado não disponível por ora.
- **Onde aparece:** `recuperacao.md`/`.html` (mapa de disparos, hoje só com e-mail; precisa passar a incluir WhatsApp nos degraus de carrinho abandonado e cartão recusado).
- **Ação:** nenhuma resposta pendente. `recuperacao.md`/`.html` precisa ser regerado (mesmo caso do item 7).

## 10. Trocar número de WhatsApp provisório do suporte

- [ ] **Status:** Aberto
- **O quê decidir:** o chat de WhatsApp de suporte a pagamentos recusados está configurado no Hotmart com o número **+55 83 99118-3123**, marcado como provisório.
- **Onde aparece:** configuração do checkout Hotmart (fora deste repositório) e qualquer menção futura ao número em `recuperacao.md`/`.html`.
- **Como resolver:** antes do lançamento oficial, troque o número no painel Hotmart pelo definitivo e me avise pra atualizar `recuperacao.md` se o número estiver citado lá.

---

*Pendências atualizadas com descobertas confirmadas direto no painel Hotmart, 25 de julho de 2026. Cheque `pendencias.html` para o checklist clicável com campo de resposta e botão "Copiar respostas pro Claude".*
