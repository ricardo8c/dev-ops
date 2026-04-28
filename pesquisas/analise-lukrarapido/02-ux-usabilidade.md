# 02 — UX & Usabilidade

## Navegação

### Menu Principal

```
Início | Sobre | Soluções | LukraRápido | LukraPay | Contato
```

| Aspecto | Avaliação |
|---------|-----------|
| Quantidade de itens | 6 itens — adequado ✅ |
| Clareza dos rótulos | Todos claros e autoexplicativos ✅ |
| ordem lógica | Sequência的自然 (Início → Sobre → Soluções → Produto → Produto → Contato) ✅ |
| Destaque do item ativo | Não identificado no snapshot |
| Hover/feedback | Não verificado |

### Breadcrumb e Estrutura

- Sem breadcrumb (site é flat, apenas uma página com scrolly)
- Estrutura simples de scrolly down — funciona mas limita profundidade

---

## Formulários

### Formulário do Hero (topo da página)

| Campo | Tipo | Obrigatório |
|-------|------|-------------|
| Seu nome | text | ✅ Sim |
| Assunto | text | ✅ Sim |
| WhatsApp | text | ❌ Não |
| Mensagem | textarea | ✅ Sim |

**Botão:** "Quero falar com a Lukra"

### Formulário LukraRápido (página do produto)

| Campo | Tipo | Obrigatório |
|-------|------|-------------|
| Seu nome | text | ✅ Sim |
| Assunto | text | ✅ Sim (preenchido: "LukraRápido - Contato") |
| Seu e-mail | email | ✅ Sim |
| WhatsApp | text | ❌ Não |
| Mensagem | textarea | ✅ Sim |

### Formulário LukraPay (página do produto)

Mesmos campos do LukraRápido (assunto pré-preenchido como "LukraPay - Contato")

### Formulário de Contato (seção footer)

| Campo | Tipo | Obrigatório |
|-------|------|-------------|
| Seu nome | text | ✅ Sim |
| WhatsApp | text | ✅ Sim |
| Assunto | text | ✅ Sim |
| Mensagem | textarea | ✅ Sim |

**Observação:** Este formulário NÃO pede e-mail, apenas WhatsApp — o que pode ser intencional (preferência por WhatsApp como canal), mas exclui leads que preferem e-mail.

---

## CTAs (Chamadas para Ação)

| Local | CTA | Avaliação |
|-------|-----|-----------|
| Hero | "Conheça a Lukra" + "Assista ao Vídeo" | 🟡 OK mas "vídeo" não existe |
| Hero | "Quero falar com a Lukra" | ✅ Bom |
| LukraPay | "Fale com a gente" (CTA secundário) | ✅ Presente |
| LukraRápido | "Fale com a gente" (CTA secundário) | ✅ Presente |
| Footer | "Fale Conosco" | ✅ Presente |
| Depoimentos | Sem CTA | ❌ Oportunidade perdida |

**Problema:** Todos os CTAs levam ao mesmo fluxo (formulário). Não há diferenciação entre "quero testar", "quero orçamento", "tenho dúvida".

---

## FAQ (Perguntas Frequentes)

### Perguntas Atuais (3)

1. "O LukraPDV é compatível com meu tipo de negócio?"
2. "Por que migrar minha maquininha para a LukraPay?"
3. "A Lukra oferece suporte técnico?"

### Avaliação do FAQ

| Aspecto | Avaliação |
|---------|-----------|
| Formato accordion | ✅ Bom — expande/clica, não sobrecarrega |
| Respostas objetivas | ✅ Bons parágrafos curtos |
| Quantidade | 🔴 Muito baixo — 3 perguntas no máximo para B2B |
| Posicionamento | ✅ Aparece após "Sobre", antes de "Soluções" |

---

## Fluxo do Usuário

### Fluxo Ideal (atual)

```
Usuário chega → Hero → Lê proposta → 
  ├─ Preenche formulário do hero (alto atrito)
  ├─ Scroll → FAQ → Lê dúvidas → 
  ├─ Scroll → Soluções → Seleciona produto →
  │   └─ Preenche formulário do produto
  ├─ Scroll → Depoimentos → LeSocial proof
  └─ Scroll → Contato → Preenche formulário
```

### Problemas do Fluxo

1. **Zero atalho para WhatsApp** — Usuário que quer resposta rápida não tem opção instantânea
2. **Formulários muito similares** — 3 formulários com campos quase idênticos confundem
3. **Sem chat ao vivo** — Nenhuma opção de conversa em tempo real
4. **Sem página de preços** — Lead que quer saber preço vai embora

---

## Mobile

| Aspecto | Avaliação |
|---------|-----------|
| Menu hamburguer | Presumido ✅ |
| Responsividade | Snapshot sugere ✅ |
| Tamanho de toque | Não verificado |
| Formulários mobile | Não verificado |

---

## Acessibilidade

| Aspecto | Status |
|---------|--------|
| Labels nos formulários | ✅ Presentes |
| Contraste | Não verificado |
| Navegação por teclado | Não verificado |
| Alt em imagens | ⚠️ "Lukra Hero Image" genérico |

---

## Nota: 7/10

> A navegação é simples e funcional, mas a falta de WhatsApp flutuante e a ausência de chat ao vivo são lacunas importantes para um produto B2B que atende por WhatsApp.