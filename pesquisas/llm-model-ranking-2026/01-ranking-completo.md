# Ranking Completo — Modelos LLM Open Weights 2026

> **Fonte dos dados:** Artificial Analysis Intelligence Index v4.0, LLM Stats, Arena AI, Hugging Face
> **Data da pesquisa:** 3 de maio de 2026

---

## 🥇 1º — gemma-4-26b-a4b (Google)

**Destaque:** Melhor custo-benefício do ranking. Surpresa geral.

| Métrica | Valor |
|---|---|
| **Intelligence Index** | **57 / 60** ⭐⭐⭐⭐ |
| Arena (Texto) | **#6** entre modelos open weights |
| Arena Chat | #98 |
| AIME 2026 | #9 (score 0.88) |
| Tool Calling (t2-bench) | #6 (0.85) |
| LiveCodeBench v6 | #19 (0.77) |
| Tipo | Reasoning + Multimodal (img + vídeo) |
| Parâmetros | 3.8B ativos / 25.2B total (MoE) |
| Contexto | 256k tokens |
| Velocidade | ~150 t/s (melhor provedor: Clarifai) |
| Custo | Input $0.13 / Output $2.85 / Cache $0.10 — ~$0.14–0.20/1M (DeepInfra) |
| Licença | Apache 2.0 ✅ |
| Lançamento | Abril 2026 |

### Pontos Fortes
- Menor ativo de todos os líderes — apenas 3.8B parâmetros ativos
- 8.4x menos parâmetros ativos que Kimi K2.5
- 43x menos parâmetros totais que Kimi K2.5
- Maior openness index (39 vs 33 do Kimi)
- Contexto multimodal (imagem + vídeo)
- Tool calling excelente (#6 no t2-bench)

### Pontos Fracos
- Output caro ($2.85/1M) — desvantagem para modelos reasoning com muito thinking
- Arena reasoning ranking baixo (#75)
- HLE (frontier knowledge): apenas 0.17 (#48)

### Quando usar
- Deploy local com recursos limitados
- Tarefas que exigem multimodalidade open weights
- Agentes com tool calling
- Melhor relação inteligência/custo

---

## 🥈 2º — kimi-k2.5 (Moonshot / Kimi)

**Destaque:** Líder em tarefas agentic open weights. Multimodal open weights.

| Métrica | Valor |
|---|---|
| **Intelligence Index** | **47 / 60** |
| GDPval-AA (agentic) | Elo **1309** — líder open weights |
| MMMU-Pro (visão) | 75% |
| AIME 2025 | #43 (score 0.90) |
| SWE-bench | ~51% (Multi-SWE) |
| Tipo | Reasoning + Multimodal (img + vídeo) |
| Parâmetros | 32B ativos / 1T total (MoE) |
| Contexto | 256k tokens |
| Velocidade | 40 t/s |
| Custo | Input $0.42 / Output $0.50 / Cache $0.20/1M |
| Licença | Modified MIT ✅ |
| Lançamento | Janeiro 2026 |

### Pontos Fortes
- **66% win rate** contra GLM-4.7 em agentic tasks
- Primeiro modelo open weights **multimodal de flagship** (img + vídeo)
- Maior contexto (256k tokens)
- Elo 1309 no GDPval-AA — próximo de modelos proprietários
- Arquitetura híbrida: reasoning on/off

### Pontos Fracos
- Velocidade baixa (40 t/s) — 3x mais lento que MiniMax
- 82M de reasoning tokens por avaliação (alto custo de output)
- HALL mark: 64% (tende a abster-se em vez de fabricar, mas ainda alto)
- Custo de output competitivo ($0.50/1M) mas não o mais barato

### Quando usar
- Tarefas agentic (automação, agentes com shell/web browsing)
- Necessidade de entrada multimodal (imagem/vídeo)
- Contextos longos (até 256k tokens)
- Melhor alternativa open weights para benchmarking contra proprietários

---

## 🥉 3º — minimax-m2.5-free (MiniMax)

**Destaque:** Velocidade impressionante por preço ínfimo. Custo-benefício para produção.

| Métrica | Valor |
|---|---|
| **Intelligence Index** | **47 / 60** (empate com Kimi!) |
| SWE-bench | 51.3% (empata com Opus em multi-file!) |
| SWE-bench Verified | #8 of 10 |
| BrowseComp | #13 |
| Tipo | Reasoning (texto only) |
| Parâmetros | 10B ativos / 230B total (MoE) |
| Contexto | 205k tokens |
| Velocidade | **119 t/s** (3x mais rápido que Kimi!) |
| Custo | Input $0.30 / Output $1.20 / Cache $0.16/1M — **FREE tier** ✅ |
| Licença | MIT ✅ |
| Lançamento | Fevereiro 2026 |

### Pontos Fortes
- **119 t/s** — #6 mais rápido entre modelos open weights
- 10B ativos (MoE) — eficiência excelente
- **Custo 1/20 do Claude Opus** para coding (SWE-bench)
- Custo 4x menor que Kimi em output tokens
- **Tier free disponível**
- Menor custo de avaliação Intelligence Index ($124.58 total)

### Pontos Fracos
- Sem suporte a imagens (texto only)
- Contexto menor (205k vs 256k do Kimi)
- 51M de reasoning tokens por avaliação (alto)

### Quando usar
- Produção com alto volume de requisições
- Coding tasks (comparável a Opus por fração do custo)
- Quando preço é fator decisivo
- **Melhor opção free tier**

---

## 4º — nvidia/nemotron-3-super-120b-a12b (NVIDIA)

**Destaque:** Melhor free tier em velocidade e contexto longo. Especializado.

| Métrica | Valor |
|---|---|
| Arena Chat | **#3** (overall!) |
| RULER (Long Context) | **#1** (0.92 @ 1M tokens!) |
| HMMT 2025 (Math) | #8 (score 0.95, with tools) |
| AIME 2025 | #43 (score 0.90) |
| GPQA (Expert QA) | 82.7 (próximo do top) |
| Tipo | Reasoning (MoE hybrid Mamba-Attention) |
| Parâmetros | 12B ativos / 120B total |
| Contexto | **1M tokens** |
| Velocidade | **218 t/s** (#2 mais rápido!) |
| Custo | **FREE tier** via API ✅ |
| Licença | NVIDIA Open Model License ✅ |
| Lançamento | Março 2026 |

### Pontos Fortes
- **#3 no Arena Chat** — entre os melhores de todos
- **1M tokens de contexto** (o único da lista)
- **218 t/s** — velocidade absurda
- #1 em RULER (128K → 1M tokens) — líder em contexto longo
- #1 em WMT24++ (tradução: 0.87)
- HMMT 2025: 0.95 com tools (#8)

### Pontos Fracos
- Coding fraco (#83 no Arena)
- Reasoning ranking baixo (#94)
- SWE-bench apenas 53.7% (vs 73% do GLM)
- BrowseComp apenas 31.3% (#41)

### Quando usar
- **Tarefas de contexto extremo** (>200k tokens)
- Tradução automática
- Matemática com ferramentas
- Free tier quando precisa de velocidade + contexto

---

## 5º — glm-4.7:cloud (Zhipu AI)

**Destaque:** Melhor para coding e output massivo. Vibe coding.

| Métrica | Valor |
|---|---|
| **Intelligence Index** | **42 / 60** |
| HLE (Frontier reasoning) | 42.8% (+12.4% vs antecessor) |
| SWE-bench (coding) | **73.8%** (melhor da lista) |
| SWE-bench Multilingual | 66.7% |
| GPQA | ~68% |
| Tipo | Reasoning (texto only) |
| Parâmetros | 32B ativos / 357B total (MoE) |
| Contexto | 200k input + **128k output** |
| Velocidade | 93 t/s |
| Custo | Input $0.60 / Output $2.20 / Cache $0.45/1M |
| Licença | MIT ✅ |
| Lançamento | Dezembro 2025 |

### Pontos Fortes
- **Melhor coding** da lista (73.8% SWE-bench)
- **128k output capacity** — gera módulos inteiros em uma chamada
- "Vibe Coding" — UI mais bonita por default
- Integração nativa com Claude Code, Cline, Roo Code
- Ótimo em HLE (42.8%)

### Pontos Fracos
- Mais verboso que a média (170M tokens output na avaliação)
- Caro para output ($2.20/1M)
- Sem multimodalidade
- Não é líder em nenhuma categoria geral

### Quando usar
- Coding agentic (princípio — resolve issues GitHub)
- Geração de código completo (múltiplos arquivos)
- Tarefas de código multilíngue
- Integração com VS Code / agentes de coding

---

## 6º — mistral-small-4 (Mistral)

**Destaque:** Melhor velocidade raw. Open weights, barato, multimodal.

| Métrica | Valor |
|---|---|
| Tipo | **Non-reasoning** (resposta direta) |
| Parâmetros | ~17B ativos / 119B total (MoE) |
| Contexto | 262k tokens |
| Velocidade | **149 t/s** (mais rápido em raw throughput!) |
| Multimodal | Sim (vision) |
| Tool Calling | ✅ |
| JSON Mode | ✅ |
| Custo | Input $0.15 / Output $0.60 / Cache $0.15/1M — **$0.26/1M blended** |
| Licença | Open weights ✅ |
| Lançamento | Março 2026 |

### Notas Importantes
- **Não é reasoning model** — não faz chain-of-thought
- Métricas de Intelligence Index **não são diretamente comparáveis**
- Se você **não precisa de raciocínio passo-a-passo**, é excelente escolha

### Pontos Fortes
- 149 t/s — velocidade máxima entre os avaliados
- Mais barato da lista ($0.26/1M blended)
- Multimodal (vision)
- Tool calling + JSON mode nativos
- Open weights (self-host)

### Pontos Fracos
- Sem reasoning — limitado para tarefas complexas
- Coding apenas razoável (~37% SWE-bench)

### Quando usar
- Tarefas rápidas e simples (sem necessidade de reasoning)
- Alto volume, baixo custo
- Necessidade de multimodalidade + tool calling
- Quando latência é crítica

---

## 7º — command-a (Cohere)

**Destaque:** Abaixo da média em quase tudo. Caro e lento.

| Métrica | Valor |
|---|---|
| **Intelligence Index** | **13 / 30** (abaixo da média!) |
| Velocidade | 39.3 t/s (abaixo da mediana de 76.6) |
| Tipo | Non-reasoning (texto only) |
| Parâmetros | 111B |
| Contexto | 256k tokens |
| Custo | Input **$2.50** / Output **$10.00**/1M — **$4.38/1M blended** |
| Verbosity | #6/30 (muito conciso — único ponto positivo) |
| Licença | CC-BY-NC 4.0 (não comercial!) ⚠️ |
| Lançamento | Março 2025 |

### Pontos Fracos
- 6.5x mais caro que a média de input
- 12.5x mais caro que a média de output
- Abaixo da média em inteligência
- Lento (39 t/s)
- CC-BY-NC (não comercial!)
- Sem multimodalidade

### Pontos Fortes
- Outputs altamente concisos (#6 em verbosity)
- Contexto 256k

### Quando usar
- Apenas para experimentation pessoal
- Não recomendado para produção ou comercial

---

## ★ — claude-sonnet-4.5 (Anthropic)

**Destaque:** Proprietário premium. Melhor coding do mundo (77.2% SWE-bench). Líder em computer use.

Claude Sonnet 4.5 possui **duas variantes** — Non-reasoning e Reasoning — ambas com multimodalidade e 1M de contexto.

### Variante Non-Reasoning

| Métrica | Valor |
|---|---|
| **Intelligence Index** | **37 / 60** (non-reasoning proprietary) |
| Arena | #14 among 70 models (well above average of 24) |
| Tipo | Non-reasoning + Multimodal (img) |
| Contexto | **1M tokens** |
| Velocidade | 47 t/s |
| Custo | Input **$3.75** / Output **$15.00** / Cache $0.30/1M |
| Blended | **$6.56/1M** (88% acima da média) |
| Latência TTFT | 1.12s (#4 mais rápido!) |
| Lançamento | 29/Set/2025 |

### Variante Reasoning (Thinking)

| Métrica | Valor |
|---|---|
| **Intelligence Index** | **43 / 60** |
| Competitors | Abaixo de GPT-5.5 (60), Opus 4.7 (57) |
| Tipo | Reasoning + Multimodal (img) |
| Contexto | **1M tokens** |
| Velocidade | 42.4 t/s (36% abaixo da mediana) |
| Custo | Input $3.75 / Output $15.00 / Cache $0.30/1M |
| Lançamento | 29/Set/2025 |

### Benchmarks Claimed (Anthropic)

| Benchmark | Score | Obs |
|---|---|---|
| SWE-bench Verified | **77.2%** | State-of-the-art |
| SWE-bench High Compute | 82.0% | Multiple attempts |
| OSWorld (computer use) | **61.4%** | Líder (+19.2pp vs 4.1) |
| MMLU | 89.2% | |
| Code Generation | 92.7% | |

### Posicionamento no Ranking

> **Importante:** Claude Sonnet 4.5 é **proprietário** — não competes diretamente com os modelos open weights do ranking. Ele está posicionado como referência de mercado.

| Métrica | Claude Sonnet 4.5 | Mejor Open Weights |
|---|---|---|
| Intelligence | 37–43/60 | gemma-4-26b: 57/60 |
| SWE-bench | 77.2% (SOTA) | glm-4.7: 73.8% |
| Computer Use | 61.4% (SOTA) | — (não disponível em open) |
| Contexto | 1M tokens | nemotron: 1M tokens |
| Custo | $6.56/1M blended | $0.20–1.00/1M |

### Pontos Fortes
- **SWE-bench 77.2%** — melhor coding do mundo
- **OSWorld 61.4%** — líder em computer use (usar PCs como humanos)
- **92% cache discount** ($0.30/1M com cache hit)
- TTFT 1.12s — latência muito baixa
- 1M tokens de contexto
- Multimodal (imagem)
- Suporte robusto a agentes (Claude Code, Agent SDK)

### Pontos Fracos
- **Proprietário** — sem acesso a weights
- Caro ($6.56/1M blended — 6x mais que gemma-4-26b)
- Lento em output (47 t/s non-reasoning, 42.4 reasoning)
- Sem suporte a imagens na versão reasoning (apenas non-reasoning)
- CC-BY-NC (não comercial para command-a)

### Quando usar
- Coding de alta complexidade (77.2% SWE-bench)
- Agentes que usam computadores (computer use)
- Tarefas que exigem contexto de 1M tokens
- Benchmark de referência para evaluation
- Quando custo não é restrição

### Nota sobre Competição
Na classe **proprietary reasoning**, Claude Sonnet 4.5 (43/60) compete com:
- GPT-5.5 (60) — líder
- Claude Opus 4.7 (57)
- Gemini 3.1 Pro (57)
- Kimi K2.6 (54)

Na classe **open weights reasoning**, o líder é gemma-4-26b (57/60) — superando até Claude Sonnet 4.5 reasoning.

---

## Resumo Comparativo

| # | Modelo | Índice | Velocidade | Custo (blended) | Multimodal | Free |
|---|---|---|---|---|---|---|
| 1 | gemma-4-26b | **57/60** | ~150 t/s | ~$0.20 | ✅ | ❌ |
| 2 | kimi-k2.5 | 47/60 | 40 t/s | ~$0.47 | ✅ | ❌ |
| 3 | minimax-m2.5 | 47/60 | **119 t/s** | ~$0.52 | ❌ | ✅ |
| 4 | nemotron-3-super | ? | **218 t/s** | **FREE** | ❌ | ✅ |
| 5 | glm-4.7 | 42/60 | 93 t/s | ~$1.00 | ❌ | ❌ |
| 6 | mistral-small-4 | N/A* | 149 t/s | **$0.26** | ✅ | ❌ |
| 7 | command-a | 13/30 | 39 t/s | $4.38 | ❌ | ❌ |
| ★ | claude-sonnet-4.5 | 37–43/60 | 42–47 t/s | $6.56 | ✅ | ❌ |

---

## Rankings por Categoria

### 🏆 Melhor Inteligência
1. gemma-4-26b (57)
2. kimi-k2.5 / minimax-m2.5 (47)
3. glm-4.7 (42)

### ⚡ Melhor Velocidade
1. nemotron-3-super (218 t/s)
2. mistral-small-4 (149 t/s)
3. gemma-4-26b (150 t/s)

### 💰 Melhor Custo-Benefício
1. gemma-4-26b ($0.20/1M + 57 de índice)
2. mistral-small-4 ($0.26/1M)
3. minimax-m2.5 ($0.52/1M + 47 de índice)

### 🎁 Melhor Free Tier
1. nemotron-3-super (218 t/s, 1M context, #3 Arena)
2. minimax-m2.5 (119 t/s, 47 de índice)

### 🎨 Melhor Coding
1. **claude-sonnet-4.5** (77.2% SWE-bench — SOTA)
2. glm-4.7 (73.8% SWE-bench)
3. kimi-k2.5
4. minimax-m2.5

### 🧠 Melhor Agentic
1. kimi-k2.5 (Elo 1309, 66% vs GLM)
2. gemma-4-26b (Tool calling #6)
3. nemotron-3-super

### 📏 Melhor Contexto Longo
1. nemotron-3-super (1M tokens, #1 RULER)
2. kimi-k2.5 (256k)
3. gemma-4-26b / mistral-small-4 (256k)

### 🖼️ Melhor Multimodal
1. kimi-k2.5 (img + vídeo)
2. gemma-4-26b (img + vídeo)
3. claude-sonnet-4.5 (img, non-reasoning only)
4. mistral-small-4 (vision)
