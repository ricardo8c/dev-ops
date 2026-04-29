# 03 — Ferramentas de Código e Programação para Sites Animados

## Frameworks, Bibliotecas e Editores

---

## ⚙️ Frameworks Front-End

### Next.js (React)
Framework React full-stack com SSR, SSG e App Router. Padrão moderno para sites animados e performáticos.

| Aspecto | Info |
|---------|-----|
| **Tecnologia** | React + Node.js |
| **Animação** | Framer Motion, GSAP, AOS |
| **Styling** | Tailwind CSS, CSS Modules |
| **Hosting** | Vercel (grátis), Netlify |
| **Performance** | SSR/SSG, image optimization |
| **Curva** | Média |
| **Melhor para** | Landing pages pro, apps |
| **URL** | nextjs. org |

### Astro
Framework orientado a conteúdo com ilhas de hidratação seletiva. Ideal para sites de conteúdo com animações isoladas.

| Aspecto | Info |
|---------|-----|
| **Tecnologia** | Multi-framework islands |
| **Animação** | Qualquer biblioteca JS |
| **Performance** | Zero JS por default |
| **Curva** | Baixa |
| **Melhor para** | Blogs, sites marketing |
| **URL** | astro. build |

### SvelteKit
Framework baseado em Svelte com compilação otimizada. Transições nativas de alto desempenho.

| Aspecto | Info |
|---------|-----|
| **Tecnologia** | Svelte (compilado) |
| **Animação** | Native transitions + Motion |
| **Performance** | Compilado (sem virtual DOM) |
| **Curva** | Baixa |
| **Melhor para** | Sites rápidos, apps |
| **URL** | svelte.dev/kit |

### Nuxt (Vue)
Framework Vue com SSR e renderização híbrida. Excelente para sites com animações complexas.

| Aspecto | Info |
|---------|-----|
| **Tecnologia** | Vue 3 + Node.js |
| **Animação** | GSAP, Three.js, Vue Motion |
| **Curva** | Média |
| **Melhor para** | Apps Vue, landing pages |
| **URL** | nuxt. com |

---

## 🎬 Bibliotecas de Animação

### Framer Motion
Biblioteca de animação mais popular para React. API declarativa, gestures, scroll e layout animations.

| Aspecto | Info |
|---------|-----|
| **Framework** | React |
| **Curva** | Baixa |
| **Features** | Scroll, gestures, layout, variants |
| **Performance** | Alta (layout animations) |
| **Preço** | Grátis (MIT) |
| **URL** | framer. com/motion |
| **Exemplo:** | `motion.div animate={{ x: 100 }}` |

### GSAP (GreenSock)
Biblioteca de animação profissional. Referência da indústria para animações web de alta performance. ScrollTrigger incluso.

| Aspecto | Info |
|---------|-----|
| **Framework** | Any (vanilla JS) |
| **Curva** | Média-alta |
| **Features** | Timeline, ScrollTrigger, plugins |
| **Performance** | Excelente |
| **Preço** | Freemium / $199/ano (Club) |
| **URL** | greensock. com |
| **Exemplo:** | `gsap.to(".box", { x: 100 })` |

### AOS (Animate on Scroll)
Biblioteca leve para animações em scroll. Simples de usar, boa para efeitos básicos.

| Aspecto | Info |
|---------|-----|
| **Framework** | Any (vanilla JS) |
| **Curva** | Muito baixa |
| **Features** | Fade, zoom, flip, parallax |
| **Performance** | Boa |
| **Preço** | Grátis (MIT) |
| **URL** | michalsnik. com/aos |
| **Exemplo:** | `data-aos="fade-up"` |

### Three.js
Biblioteca WebGL para gráficos 3D no navegador. Altíssima curva, altíssimo impacto.

| Aspecto | Info |
|---------|-----|
| **Framework** | Vanilla JS |
| **Curva** | Alta |
| **Features** | 3D, shaders, física, partículas |
| **Performance** | GPU (WebGL) |
| **Preço** | Grátis (MIT) |
| **URL** | threejs. org |
| **Melhor para** | Experiências imersivas |

### Anime.js
Biblioteca de animação vanilla JS leve e flexível. Boa alternativa ao GSAP para projetos menores.

| Aspecto | Info |
|---------|-----|
| **Framework** | Vanilla JS |
| **Curva** | Baixa |
| **Features** | Timeline, easing, callbacks |
| **Performance** | Boa |
| **Preço** | Grátis (MIT) |
| **URL** | animejs. com |
| **Exemplo:** | `anime({ targets: '.box', translateX: 100 })` |

### Lenis (Smooth Scroll)
Biblioteca de scroll suave moderno. Substitui o Locomotive Scroll. Funciona com qualquer biblioteca de animação.

| Aspecto | Info |
|---------|-----|
| **Framework** | Vanilla JS |
| **Curva** | Baixa |
| **Features** | Smooth scroll, integração GSAP/Framer |
| **Performance** | Excelente |
| **Preço** | Grátis |
| **URL** | lenis. studio |
| **Exemplo:** | `lenis. smooth()` |

### Motion One
Biblioteca de animação pequena (~3KB). Alternativa minimalista ao Framer Motion.

| Aspecto | Info |
|---------|-----|
| **Framework** | Vanilla JS ou React |
| **Curva** | Baixa |
| **Features** | Web Animations API wrapper |
| **Performance** | Ótima |
| **Preço** | Grátis (MIT) |
| **URL** | motion one. dev |

### Spline (spline. scene)
Editor visual 3D para criar cenas interativas. Exporta para web como runtime WebGL.

| Aspecto | Info |
|---------|-----|
| **Framework** | Editor visual |
| **Curva** | Baixa (editor) |
| **Features** | Editor visual, 3D interativo |
| **Performance** | Boa |
| **Preço** | Freemium |
| **URL** | spline. scene |

---

## 🛠️ Editores com AI

### Cursor
Editor VS Code-based com AI integrada (Windsurf, Claude Code, Copilot). Permite geração de código animado via chat.

| Aspecto | Info |
|---------|-----|
| **Modelo AI** | Claude (Windsurf) ou Copilot |
| **Curva** | Baixa |
| **Features** | Chat-to-code, autocomplete, debug |
| **Preço** | Freemium / $20/mês (Pro) |
| **Melhor para** | Desenvolvedores |
| **URL** | cursor. com |

### Replit Agent
Agente AI que gera código completo a partir de prompts em linguagem natural. Executa e deploya automaticamente.

| Aspecto | Info |
|---------|-----|
| **Modelo AI** | Gemini |
| **Curva** | Muito baixa |
| **Features** | Geração completa, deploy, banco de dados |
| **Preço** | Freemium |
| **Melhor para** | Não-codificadores |
| **URL** | replit. com |

### Windsurf (Codeium)
Editor com AI agent de nova geração. Memória de projeto, contexto longo, automação.

| Aspecto | Info |
|---------|-----|
| **Modelo AI** | Codeium (Claude-based) |
| **Curva** | Baixa |
| **Features** | Agent mode, Cascade, autocomplete |
| **Preço** | Freemium / $10/mês (Pro) |
| **Melhor para** | Desenvolvedores |
| **URL** | codeium. com/windsurf |

### VS Code + Copilot
Editor referência + AI completions. Extensões para animação (Framer Motion snippets, Tailwind AI).

| Aspecto | Info |
|---------|-----|
| **Modelo AI** | OpenAI GPT-4o |
| **Curva** | Baixa |
| **Features** | Autocomplete, chat, review |
| **Preço** | $10-19/mês |
| **Melhor para** | Desenvolvedores |
| **URL** | code.visualstudio.com |

---

## 🎯 Stack Recomendado por Perfil

| Perfil | Stack | Ferramenta AI |
|--------|-------|---------------|
| **Não-codificador** | Wix ADI / Framer | DesignRocket tutorials |
| **Designer** | Framer / Dora | Framer AI |
| **Frontend Junior** | Astro + AOS | Cursor / Windsurf |
| **Frontend Sênior** | Next.js + Framer Motion | Cursor |
| **Full-stack** | Next.js + GSAP + Lenis | Replit Agent / Cursor |
| **3D/Imersivo** | Next.js + Three.js + Spline | Cursor |
| **Agilidade** | Astro + Tailwind + Motion One | Windsurf |