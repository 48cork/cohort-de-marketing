[← Book do Funil](../index.html)

# Mockups de Produto: Pesquisador Aumentado™

**Skill:** `/mockup-produto-funil`
**Data:** 25 de julho de 2026
**Fonte dos itens:** `offerbook.md` BLOCO 2 (produto, módulos, isca digital, bônus)
**Fonte da identidade visual:** `DESIGN.md` (cores, fontes, raio de borda, tom visual)
**Status:** Prompts prontos pra gerar. Esta skill não gera imagem nem publica: você gera na ferramenta de sua escolha e aprova.

---

## Mapa de tokens usados (do seu DESIGN.md)

| Token | Valor | Uso nos prompts |
|---|---|---|
| `{{cor-fundo}}` | `#faf9f5` (cream quente) | Fundo liso de todos os mockups |
| `{{cor-primaria}}` | `#141413` (tinta quase preta) | Título, texto principal, cor de ação dominante (a mesma usada nos botões do DESIGN.md) |
| `{{cor-secundaria}}` | `#d97757` (terracota) | Acento/marca apenas, nunca preenchimento sólido (regra do seu DESIGN.md: terracota só marca, não preenche superfície) |
| `{{cor-texto}}` | `#5e5d59` (cinza-morno) | Subtítulo, texto secundário |
| `{{fonte-titulo}}` | system-ui, peso 700, tracking negativo (-0.02em a -0.03em) | Títulos e nome do produto |
| `{{fonte-corpo}}` | system-ui, peso 400 | Corpo/legendas dentro das telas |
| `{{raio-borda}}` | `4px` (botões) / `8px` (cards) | Cantos de cards, telas, botões |
| `{{estilo-visual}}` | Editorial minimalista: cream + tinta quase preta, terracota só como acento (nunca preenchimento), zero gradiente, sombra de estúdio suave só pra dar volume 3D ao mockup | Tom geral de toda a família de mockups |
| `{{logo-ou-marca}}` | Wordmark "Pesquisador Aumentado™", com o "A" de "Aumentado" destacado em terracota (`#d97757`) | Marca em cada peça |

**Itens do offerbook mockupados nesta rodada:**
- Produto principal: e-book **Pesquisador Aumentado™** (introdução + 5 capítulos)
- Isca digital: **"As 7 Perguntas Socráticas que Todo Orientador Deveria Fazer Antes de Qualquer Sessão de TCC"** (já escrita em `isca-7-perguntas-socraticas.md`)

**Item deixado de fora:** o bônus de lançamento pago ainda não foi definido pelo dono da oferta (pendência 1 em `pendencias.md`). Sem o item existir no offerbook, não há o que mockupar. Quando for definido, rode esta skill de novo só para esse item.

---

## 1. Capa de ebook — Produto principal

**Tipo:** Capa de ebook / PDF
**Por quê:** o produto principal é entregue como e-book; capa dá "cara de livro" e é a peça mais usada na página de vendas.

```
Mockup de capa de ebook 3D, em pé, vista frontal levemente em ângulo, fundo #faf9f5 liso.
Título "Pesquisador Aumentado" em destaque, tipografia system-ui peso 700 com tracking
negativo (-0.02em), na cor #141413. O "A" de "Aumentado" destacado na cor #d97757.
Subtítulo "O Método Socrático com IA para Professores Orientadores de TCC" menor, na
cor #5e5d59.
Um único acento gráfico na cor #d97757 (linha ou marca, nunca preenchimento sólido).
Marca "Pesquisador Aumentado™" no rodapé da capa.
Estilo visual geral: editorial minimalista, cream quente + tinta quase preta, zero
gradiente, terracota usado só como marca. Iluminação de estúdio suave, sombra realista
no chão.
Sem texto extra, sem marca-d'água, alta resolução, proporção vertical de livro.
```

---

## 2. Box do produto — Produto principal

**Tipo:** Box / caixa do produto
**Por quê:** ancora o e-book (produto 100% digital) como algo de valor físico percebido, pra página de vendas e criativos de anúncio.

```
Mockup de caixa de produto 3D, fechada, vista frontal em ângulo, sobre superfície
neutra, fundo #faf9f5.
A caixa estampa o título "Pesquisador Aumentado™" em tipografia system-ui peso 700,
tracking negativo, na cor #141413, com o "A" de "Aumentado" destacado em #d97757.
Acabamento fosco, sem brilho, coerente com um estilo editorial minimalista (não usar
verniz espelhado nem gradiente colorido).
Acento gráfico na cor #d97757 usado apenas como uma linha ou marca fina, nunca como
preenchimento da caixa.
Iluminação de estúdio, reflexo e sombra realistas. Proporção de caixa de produto,
alta resolução, sem texto extra.
```

---

## 3. Device mockup — Índice do e-book

**Tipo:** Device mockup
**Por quê:** o produto é um e-book em PDF, não uma plataforma de curso com área de membros. Por honestidade com o que a oferta realmente é, este mockup mostra o **e-book aberto num tablet/notebook exibindo o índice** (introdução + 5 capítulos), não uma "área de membros" que não existe.

```
Mockup de tablet exibindo a tela de um e-book em PDF aberto, vista frontal, fundo #faf9f5
liso.
Na tela, um índice/sumário visível com os itens: "Introdução", "Capítulo 1: O Problema
Estrutural", "Capítulo 2: Metodologia Socrática Aplicada", "Capítulo 3: IA como
Interlocutor Socrático", "Capítulo 4: Protocolo de Orientação em 3 Camadas",
"Capítulo 5: Implementação Imediata".
Cada item do índice em tipografia system-ui, cor #141413, com o número do capítulo em
#d97757. Cabeçalho da tela com a marca "Pesquisador Aumentado™" na cor #141413.
Cantos da tela do device com raio de 8px. Estilo visual: editorial minimalista, sem
gradiente, terracota só como acento.
Device centralizado, iluminação suave, sombra realista. Alta resolução, sem texto
fora da tela.
```

---

## 4. Capa da isca digital — "7 Perguntas Socráticas"

**Tipo:** Capa de ebook / PDF (versão mais leve, 1 página)
**Por quê:** a isca já tem o conteúdo escrito (`isca-7-perguntas-socraticas.md`); o mockup dá a ela a mesma "cara de material" do produto principal, mas mais simples, coerente com ser gratuita e curta.

```
Mockup de folha/PDF de 1 página, vista frontal quase reta (sem ângulo de livro grosso,
já que é um guia de 1 página, não um ebook espesso), fundo #faf9f5 liso.
Título "As 7 Perguntas Socráticas que Todo Orientador Deveria Fazer Antes de Qualquer
Sessão de TCC" em tipografia system-ui peso 700, tracking negativo, na cor #141413,
quebrado em até 3 linhas.
Etiqueta pequena acima do título, uppercase, tracking bem aberto, na cor #d97757,
com o texto "ISCA DIGITAL · MÉTODO SOCRÁTICO COM IA".
Marca "Pesquisador Aumentado™" no rodapé, com o "A" de "Aumentado" em #d97757.
Estilo visual: editorial minimalista, mesma família visual do produto principal mas
mais leve (menos elementos, mais espaço em branco).
Iluminação de estúdio suave, sombra sutil de papel (não de livro grosso). Alta
resolução, proporção de folha A4/Letter, sem marca-d'água.
```

---

## 5. Bundle de bônus empilhado — Produto + isca

**Tipo:** Bundle de bônus empilhado
**Por quê:** mostra o que o professor recebe de uma vez (produto principal + isca), reforçando volume e valor. O bônus de lançamento pago fica de fora até ser definido.

```
Mockup de bundle/kit: composição com 2 elementos agrupados e levemente sobrepostos —
1 box de produto fechado com o título "Pesquisador Aumentado™" e 1 folha/PDF de 1
página com o título "As 7 Perguntas Socráticas...", ambos com a mesma identidade:
cor de destaque #141413, acento #d97757 usado só como marca, fundo #faf9f5, tipografia
system-ui peso 700 nos títulos, marca "Pesquisador Aumentado™" visível em cada peça.
Composição organizada mostrando volume e valor ("tudo que vem junto"), sem
sobreposição que esconda os títulos. Estilo visual: editorial minimalista, zero
gradiente, sombras de estúdio suaves e realistas.
Alta resolução, sem texto solto fora das peças, sem marca-d'água.

Nota: quando o bônus de lançamento pago for definido (pendência 1 em pendencias.md),
adicionar um terceiro elemento a este bundle mantendo os mesmos tokens de cor e fonte.
```

---

## Checklist de qualidade (rodar depois de gerar cada imagem)

**Legibilidade**
- [ ] Título do produto/isca legível, sem corte, sem fundo de baixo contraste
- [ ] Nenhum texto saiu borrado/deformado pelo gerador (refazer se ilegível)

**Fidelidade à marca**
- [ ] Cor primária `#141413` e acento `#d97757` batem com o `DESIGN.md` (não são cores que o gerador inventou)
- [ ] Terracota aparece só como marca/acento, nunca como preenchimento sólido de superfície (regra explícita do seu DESIGN.md)
- [ ] Tipografia lembra system-ui com tracking negativo nos títulos
- [ ] A marca "Pesquisador Aumentado™" aparece corretamente em cada peça

**Consistência entre mockups**
- [ ] Os 5 mockups usam a mesma paleta e fonte (família de produtos, não peças soltas)
- [ ] Fundo, iluminação e ângulo coerentes entre as peças

**Aderência ao offerbook**
- [ ] Os 5 capítulos do índice (mockup 3) batem com a estrutura real do e-book (offerbook.md BLOCO 2)
- [ ] Nenhum bônus inventado entrou no bundle: só produto principal + isca confirmada

---

## Próximos passos

1. Gerar as 5 imagens na ferramenta de geração de imagem de sua escolha, usando os prompts acima.
2. Rodar o checklist de qualidade em cada uma.
3. Quando o bônus de lançamento pago for definido (pendência 1), voltar aqui pra adicionar o mockup dele ao bundle.
4. Usar as imagens aprovadas na página de vendas (quando ela existir) e nos criativos de anúncio.

---

*Mockups gerados por `/mockup-produto-funil`, lendo `offerbook.md` (itens) e `DESIGN.md` (identidade visual). A skill entrega os prompts; a geração da imagem e a aprovação são suas.*
