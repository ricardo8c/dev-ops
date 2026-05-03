# Tabela Comparativa — Modelos LLM Open Weights 2026

> Comparação lado a lado dos modelos avaliados. Dados de Artificial Analysis Intelligence Index, Arena AI, LLM Stats, Hugging Face.

---

## Especificações Técnicas

| Modelo | Provider | Parâmetros (Ativos/Total) | Contexto | Multimodal | Reasoning | Lançamento |
|--------|----------|---------------------------|----------|------------|-----------|------------|
| gemma-4-26b | Google | 3.8B / 25.2B (MoE) | 256k | ✅ img+vídeo | ✅ | Abr 2026 |
| kimi-k2.5 | Moonshot | 32B / 1T (MoE) | 256k | ✅ img+vídeo | ✅ | Jan 2026 |
| minimax-m2.5 | MiniMax | 10B / 230B (MoE) | 205k | ❌ | ✅ | Fev 2026 |
| nemotron-3-super | NVIDIA | 12B / 120B (MoE) | **1M** | ❌ | ✅ | Mar 2026 |
| glm-4.7 | Zhipu AI | 32B / 357B (MoE) | 200k+128k | ❌ | ✅ | Dez 2025 |
| mistral-small-4 | Mistral | ~17B / 119B (MoE) | 262k | ✅ vision | ❌ | Mar 2026 |
| command-a | Cohere | 111B | 256k | ❌ | ❌ | Mar 2025 |

---

## Performance

| Modelo | Intelligence Index | Arena Chat | Arena Coding | Arena Vision |
|--------|-------------------|------------|--------------|--------------|
| gemma-4-26b | **57/60** ⭐ | #98 | — | #56 |
| kimi-k2.5 | 47/60 | — | — | #75 (MMMU-Pro) |
| minimax-m2.5 | 47/60 | — | #12 (SWE) | — |
| nemotron-3-super | ? | **#3** | #83 | #62 |
| glm-4.7 | 42/60 | — | **73.8%** (SWE-bench) | — |
| mistral-small-4 | N/A* | — | ~37% | — |
| command-a | 13/30 | — | — | — |

*Non-reasoning — métrica não comparável*

---

## Benchmarks-Chave

| Modelo | HLE (Reasoning) | SWE-bench (Coding) | AIME (Math) | GPQA (Expert) | RULER (Context) |
|--------|----------------|--------------------|-------------|---------------|-----------------|
| gemma-4-26b | 0.17 (#48) | 0.77 (#19) | 0.88 (#9) | 0.82 | — |
| kimi-k2.5 | — | ~51% | 0.90 (#43) | — | — |
| minimax-m2.5 | — | 51.3% | — | — | — |
| nemotron-3-super | 0.23 (#38) | 53.7% | 0.90 (#43) | **82.7** | **0.92 @1M (#1)** |
| glm-4.7 | **42.8%** | **73.8%** | — | ~68% | — |
| mistral-small-4 | N/A | ~37% | — | — | — |
| command-a | N/A | — | — | — | — |

---

## Velocidade e Custo

| Modelo | Velocidade (t/s) | Input $/1M | Output $/1M | Cache $/1M | Blended $/1M | Free Tier |
|--------|-----------------|-----------|------------|-----------|--------------|-----------|
| gemma-4-26b | ~150 | $0.13 | $2.85 | $0.10 | ~$0.20 | ❌ |
| kimi-k2.5 | 40 | $0.42 | $0.50 | $0.20 | ~$0.47 | ❌ |
| minimax-m2.5 | **119** | $0.30 | $1.20 | $0.16 | ~$0.52 | ✅ |
| nemotron-3-super | **218** | — | — | — | **FREE** | ✅ |
| glm-4.7 | 93 | $0.60 | $2.20 | $0.45 | ~$1.00 | ❌ |
| mistral-small-4 | 149 | $0.15 | $0.60 | $0.15 | **$0.26** | ❌ |
| command-a | 39 | **$2.50** | **$10.00** | — | $4.38 | ❌ |

---

## Licenças e Disponibilidade

| Modelo | Licença | Comercial | Self-Host | Open Weights | API Free |
|--------|---------|-----------|-----------|--------------|----------|
| gemma-4-26b | Apache 2.0 | ✅ | ✅ | ✅ | ❌ |
| kimi-k2.5 | Modified MIT | ✅ | ✅ | ✅ | ❌ |
| minimax-m2.5 | MIT | ✅ | ✅ | ✅ | ✅ |
| nemotron-3-super | NVIDIA Open | ✅ | ✅ | ✅ | ✅ |
| glm-4.7 | MIT | ✅ | ✅ | ✅ | ❌ |
| mistral-small-4 | Open Weights | ✅ | ✅ | ✅ | ❌ |
| command-a | CC-BY-NC 4.0 | ❌ | ✅ | ✅ | ❌ |

---

## Casos de Uso Recomendados

| Modelo | Melhor Para | Evitar Para |
|--------|------------|------------|
| gemma-4-26b | Local/deploy limitado, tool calling, multimodal | Tarefas que precisam de muito output reasoning |
| kimi-k2.5 | Agentes complexos, multimodal, benchmark open weights | Budget apertado, alta velocidade |
| minimax-m2.5 | Produção em escala, coding, melhor free tier | Necessidade de imagens |
| nemotron-3-super | Contexto longo (>200k), tradução, matemática | Coding, tarefas generalistas |
| glm-4.7 | Coding agentic, código multilíngue, output longo | Tarefas multimodais |
| mistral-small-4 | Tarefas simples, alto volume, multimodal | Raciocínio complexo |
| command-a | Experimentação pessoal | Produção, qualquer uso comercial |

---

## Visual Ranking (por Intelligence Index)

```
Destaque     gemma-4-26b                    ████████████████████████████ 57/60
Top Open     kimi-k2.5 / minimax-m2.5       ████████████████████████░░░░ 47/60
Bom          glm-4.7                        ██████████████████░░░░░░░░░ 42/60
N/A*         mistral-small-4                — (não comparável)
Baixo        command-a                      ██████████░░░░░░░░░░░░░░░░░░ 13/30
```

---

## Quick Decision Tree

```
Precisa multimodal?
├─ SIM → gemma-4-26b (custo) vs kimi-k2.5 (agentes)
└─ NÃO
   ├─ Precisa de contexto EXTREMO (>200k tokens)?
   │  └─ SIM → nemotron-3-super (FREE, 1M, 218 t/s)
   ├─ Precisa de coding melhor?
   │  └─ SIM → glm-4.7 (73.8% SWE-bench)
   ├─ Prioridade é preço?
   │  └─ SIM → minimax-m2.5 (FREE tier, $0.52 blended)
   └─ Prioridade é velocidade + simplicidade?
      └─ SIM → mistral-small-4 ($0.26/1M, 149 t/s)
```
