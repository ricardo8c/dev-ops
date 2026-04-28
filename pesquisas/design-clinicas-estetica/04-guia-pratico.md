# Guia Prático — Do Conceito ao Site

> Roteiro completo para construir um site profissional para clínicas de estética, beleza e cabelo. Desde a escolha da plataforma até o lançamento e manutenção.

---

## 🗺️ Roadmap de Desenvolvimento

```
Semana 1-2     → Planejamento e Conteúdo
Semana 3-4     → Design e Protótipo
Semana 5-8     → Desenvolvimento
Semana 9       → Testes e Ajustes
Semana 10      → Lançamento
Ongoing        → SEO, manutenção e迭代
```

---

## 📋 Fase 1: Planejamento (Semana 1-2)

### 1.1 Defina Seu Posicionamento

Responda antes de começar:

| Pergunta | Responda |
|----------|----------|
| Qual seu público-alvo? | (ex: mulheres 25-45, homens que cuidam da barba) |
| Qual faixa de preço? | (ex: acessível, médio, premium) |
| Qual seu diferencial? | (ex: técnica exclusiva, horário flexível, localização) |
| Quais serviços principais? | Liste todos |
| Você tem múltiplas localizações? | (sim/não) |

### 1.2 Organize o Conteúdo

Documente ANTES de começar a construir:

**Para cada serviço:**
- [ ] Nome do serviço
- [ ] Descrição (2-3 frases)
- [ ] Para quem é indicado
- [ ] Duração típica
- [ ] Faixa de preço
- [ ] Fotos de antes/depois (mínimo 3 por serviço)
- [ ] FAQ (3 perguntas comuns)

**Para cada profissional:**
- [ ] Nome completo
- [ ] Cargo/Função
- [ ] Foto profissional (alta resolução)
- [ ] Mini bio (2-3 frases)
- [ ] Formação/Certificações
- [ ] Especialidades
- [ ] Redes sociais (se tiver)

**Para a clínica:**
- [ ] História/sobre
- [ ] Diferenciais
- [ ] Fotos do ambiente (mínimo 10)
- [ ] Endereço completo
- [ ] Horários de funcionamento
- [ ] Redes sociais

### 1.3 Defina a Estrutura de Páginas

**Estrutura mínima (5 páginas):**
```
Home          → Hero + Serviços + Agendamento
Serviços      → Lista + Descrição detalhada
Galeria       → Antes/Depois + Fotos do ambiente
Sobre/Nós     → História + Equipe
Contato       → Formulário + Mapa + Informações
```

**Estrutura completa (8-10 páginas):**
```
Home
├── hero + CTA rápido para agendamento
├── serviços destacados
├── galeria rápida
├── depoimentos
└── CTA final

/servicos
├── lista completa
├── filtros por categoria
└── cada serviço com página dedicada

/galeria
├── antes/depois
├── fotos do ambiente
└── vídeos

/sobre
├── história da clínica
├── equipe
└── certificações

/contato
├── formulário
├── mapa
├── horários
└── WhatsApp

/blog (opcional)
└── artigos educativos

/agendar
├── widget de agendamento
└── instruções
```

---

## 🖥️ Fase 2: Escolha da Plataforma

### Opção A: Construtores DIY (Rápido e Barato)

| Plataforma | Custo | Melhor Para |
|------------|-------|-------------|
| **Wix** | R$ 27-80/mês | Agilidade, templates prontos |
| **Squarespace** | R$ 27-60/mês | Design premium, beleza |
| **WordPress.com** | R$ 15-50/mês | Controle, SEO |
| **Canva** | Grátis / R$ 13-50/mês | Templates prontos, fácil |

**Prós:** Rápido, barato, sem código  
**Contras:** Limitado em personalização, dependência da plataforma

---

### Opção B: WordPress.org (Equilíbrio)

| Item | Custo Estimado |
|------|----------------|
| Hosting (Cloudflare/WP Engine) | R$ 30-100/mês |
| Tema (Elementor Pro / Divi) | R$ 100-200/ano |
| Plugin de agendamento | R$ 30-100/ano |
| SSL | Grátis (Cloudflare) ou ~R$ 100/ano |
| Desenvolvimento (se terceirizar) | R$ 3.000-10.000 |
| **Total ano 1** | **R$ 3.500-15.000** |
| **Manutenção/ano** | **R$ 1.500-5.000** |

**Prós:** Controle total, melhor SEO, integrações flexíveis  
**Contras:** Necessita manutenção, curva de aprendizado

---

### Opção C: Desenvolvimento Customizado (Premium)

- Custo: R$ 10.000-50.000+
- Indicado para: múltiplas clínicas, necessidades únicas, integração com sistemas existentes
- Stack típico: Next.js + Headless CMS (Contentful, Strapi) + Vercel/Cloudflare

**Prós:** Totalmente customizável, escalável, único  
**Contras:** Caro, tempo de desenvolvimento longo

---

## 🎨 Fase 3: Design

### Checklist Visual

**Paleta de cores:**
- [ ] Cor primária (ex: rosa blush #F4C2C2)
- [ ] Cor secundária (ex: dourado champanhe #C9A96E)
- [ ] Cor de fundo (ex: off-white #F9F7F4)
- [ ] Cor de texto (ex: charcoal #333333)
- [ ] Cor de CTA/botões (ex: rose gold)

**Tipografia:**
- [ ] Fonte para títulos (serifada ou display)
- [ ] Fonte para corpo (sans-serif legível)
- [ ] Escala tipográfica (H1, H2, H3, body, caption)

**Elementos gráficos:**
- [ ] Logo em alta resolução
- [ ] Ícones (ex: Phosphor Icons, Lucide)
- [ ] Padrões/texturas (se aplicável)
- [ ] Linha gráfica consistente

### Protótipo
1. Wireframe no papel ou Figma (baixa fidelidade)
2. Design de alta fidelidade
3. Teste com usuários reais (pelo menos 3 pessoas)
4. Ajustes baseados em feedback

---

## ⚙️ Fase 4: Desenvolvimento Técnico

### Checklist de Implementação

#### Performance
- [ ] Imagens em WebP com fallback
- [ ] Lazy loading de imagens
- [ ] CDN configurado (Cloudflare)
- [ ] Minificação de CSS/JS
- [ ] Core Web Vitals otimizados
  - LCP < 2.5s
  - FID < 100ms
  - CLS < 0.1
- [ ] Tempo de carregamento < 3s mobile

#### SEO On-Page
- [ ] Meta titles e descriptions únicos por página
- [ ] Tags H1 (uma por página), H2, H3 hierárquicos
- [ ] URLs amigáveis (ex: /servicos/botox-capilar)
- [ ] Alt text em todas as imagens
- [ ] Schema markup (LocalBusiness, Service, Review)
- [ ] Sitemap.xml gerado
- [ ] robots.txt configurado
- [ ] Canonical URLs

#### Segurança (essencial no Brasil — LGPD)
- [ ] HTTPS (SSL) ativado
- [ ] Política de privacidade
- [ ] Terms de uso (se coleta dados)
- [ ] Cookie consent banner
- [ ] Backup automático
- [ ] Atualizações de segurança em dia

#### Acessibilidade
- [ ] Contraste de cores adequado
- [ ] Navegação por teclado funcional
- [ ] Labels em todos os formulários
- [ ] Alt text em imagens
- [ ] Áudio transcrito (se aplicável)

---

## 🚀 Fase 5: Lançamento

### Pré-lançamento
- [ ] Testar em múltiplos dispositivos (iOS, Android, desktop)
- [ ] Testar todos os formulários (enviar testes reais)
- [ ] Testar agendamento end-to-end
- [ ] Validar links (sem links quebrados)
- [ ] Verificar em múltiplos navegadores
- [ ] Speed test (PageSpeed Insights)
- [ ] SEO audit ( Screaming Frog ou similar)

### Dia do Lançamento
- [ ] DNS propagado
- [ ] Analytics configurado (GA4)
- [ ] Google Search Console verificado
- [ ] Google Business Profile atualizado com link para site
- [ ] Notificar redes sociais
- [ ] Announcement para lista de emails

---

## 📈 Fase 6: Manutenção e Crescimento

### Diário
- Monitorar agendamentos
- Responder mensagens (WhatsApp/chat)
- Verificar emails

### Semanal
- Postar nas redes sociais com link para o site
- Atualizar fotos/serviços se necessário
- Verificar avaliações (Google, redes)

### Mensal
- Revisar performance (GA4: tráfego, conversões)
- Postar no blog (se tiver)
- Testar todos os formulários e links
- Verificar velocidade do site
- Atualizar preços se necessário

### Trimestral
- Análise de SEO (ranking, palavras-chave)
- A/B test de headlines ou CTAs
- Revisar concorrentes
- Atualizar fotos da equipe e galeria
- Backup e segurança: checar integridade

---

## 🛠️ Ferramentas Recomendadas

### Design
- **Figma** — Prototipagem e design
- **Canva** — Imagens rápidas e posts
- **Unsplash / Pexels** — Fotos de banco (como fallback)

### Desenvolvimento
- **WordPress + Elementor** — Construção
- **Cloudflare** — CDN, SSL, segurança
- **WP Engine** — Hosting WordPress otimizado
- **Vercel** — Hospedagem de sites estáticos

### Agendamento
- **Calendly** — Agendamento gratuito (básico)
- **Acuity** — Agendamento robusto
- **Booksy** — Focado em beleza/salões
- **Gendo / Anolla** — Soluções brasileiras

### Marketing
- **Mailchimp / RD Station** — Email marketing
- **HubSpot** — CRM completo
- **Hotjar** — Mapas de calor e gravações
- **Google Analytics 4** — Análise de tráfego

### SEO
- **Google Search Console** — Performance de busca
- **SEMrush / Ahrefs** — Análise competitiva
- **Yoast / RankMath** — SEO on-page (WordPress)

---

## 💰 Estimativa de Investimento

| Tipo | Básico | Intermediário | Premium |
|------|--------|----------------|---------|
| **Plataforma** | Canva/Wix (R$ 15-30/mês) | WordPress (R$ 100-200/mês) | Customizado |
| **Design** | Templates prontos | Tema customizado | Designer dedicado |
| **Desenvolvimento** | DIY | Freelancer/Agência | Time dedicado |
| **Ano 1** | **R$ 500-2.000** | **R$ 5.000-20.000** | **R$ 30.000-100.000** |
| **Manutenção/ano** | **R$ 200-500** | **R$ 2.000-8.000** | **R$ 10.000-30.000** |

---

*Última atualização: 26/04/2026*