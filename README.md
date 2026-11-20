#### Neurotracer AI

[](/url?sa=i&source=web&rct=j&url=https://doi.org/10.5281/zenodo.24341954&ved=2ahUKEwij8a3-_pWYAxXvKBAIHc2dNSIQy_kOegYIAAgSEAg&opi=89978449&cd&psig=AOvVaw3bOUoMsnZ2aTQ2oQZ9Y_nP&ust=1795245019025000)
[](/url?sa=i&source=web&rct=j&url=https://opensource.org/licenses/Apache-2.0&ved=2ahUKEwij8a3-_pWYAxXvKBAIHc2dNSIQy_kOegYIAAgSEAk&opi=89978449&cd&psig=AOvVaw3bOUoMsnZ2aTQ2oQZ9Y_nP&ust=1795245019025000)
[](/url?sa=i&source=web&rct=j&url=https://www.python.org/downloads/&ved=2ahUKEwij8a3-_pWYAxXvKBAIHc2dNSIQy_kOegYIAAgSEAo&opi=89978449&cd&psig=AOvVaw3bOUoMsnZ2aTQ2oQZ9Y_nP&ust=1795245019025000) 

**Neurotracer AI** is a methodology and architectural framework aimed at preserving human meaning, ensuring verifiable interpretation, and enforcing safe autonomous AI agent control in cross-lingual environments. 

**Core Principle:** *AI traces connections across fragmented signals; humans remain the authors of meaning.* 

#### Overview

In the era of ubiquitous machine translation and multi-agent ecosystems (*Agentic Web*), a critical trust gap emerges between human-expressed meaning and machine execution. During translation, paraphrasing, and delegation across chains of autonomous agents, original constraints can be distorted, replaced by algorithmic assumptions, or exploited to conceal adversarial intent. 

**Neurotracer AI** addresses this by constructing a coherent **Verifiable Interpretation Graph** G = (V, E) that strictly separates: 

1. **Raw Human Expression** (

Irawcap I sub raw end-sub
𝐼raw
⁠)
2. **Machine-Generated Hypothesis** (

Ihypcap I sub hyp end-sub
𝐼hyp
⁠)
3. **Human-Confirmed Intent** (

Iconfcap I sub conf end-sub
𝐼conf
⁠)
4. **Safety-Cleared Executable Goal** (

Iexeccap I sub exec end-sub
𝐼exec
⁠)

#### Dual-Gate Governance

Execution by an autonomous agent is permitted only when both authenticity/meaning integrity (

τauthtau sub auth end-sub
𝜏auth
⁠) and third-party non-harm safety invariants (

τsafetau sub safe end-sub
𝜏safe
⁠) satisfy domain thresholds: 

Execute⟺(τauth≥θauth)∧(τsafe≥θsafe)Execute ⟺ open paren tau sub auth end-sub is greater than or equal to theta sub auth end-sub close paren space logical and space open paren tau sub safe end-sub is greater than or equal to theta sub safe end-sub close paren
Execute⟺(𝜏auth≥𝜃auth)∧(𝜏safe≥𝜃safe)
 

#### Repository Structure

Показать код

Скрыть код

Скачать диаграмму в формате SVG

ASCII

neurotracer-ai/
├── neurotracer_core.py   # Reference implementation of Dual-Gate Engine & 5-case evaluation suite
├── LICENSE               # Apache License 2.0
└── README.md             # Architecture overview, documentation, and citation metadata

Используйте код с осторожностью.

Скопировать код в буфер обмена.

#### Quick Start

The reference prototype requires **Python 3.9+** and uses only the Python standard library (zero external dependencies). 

bash

git clone https://github.com/Neurotracer/neurotracer-ai.git
cd neurotracer-ai
python neurotracer_core.py

Используйте код с осторожностью.

Скопировать код в буфер обмена.

#### Included Stress-Test Scenarios

* **Case 1 (Cross-Lingual Translation Noise):** Preserves valid B2B intent and executes action despite severe machine translation distortion.
* **Case 2 (Multi-Agent Meaning Drift):** Halts execution when an intermediate agent drops an explicit authorial prohibition (no_public_share).
* **Case 3 (Ambiguous Instruction):** Triggers a clarification loop (REQUEST_CLARIFICATION) instead of silently guessing missing parameters.
* **Case 4 (VIP Spoofing & Prompt Injection):** Blocks session hijacking and embedded [SYSTEM NOTE] overrides via the authenticity gate (

τauthtau sub auth end-sub
𝜏auth
⁠).
* **Case 5 (Authenticated Destructive Intent):** Blocks third-party harm via the non-harm gate (

τsafetau sub safe end-sub
𝜏safe
⁠) while logging auditable author accountability in the graph.

#### Mechanistic Verification (Gemma-2-2B)

Ontology coherence was verified via Circuit Tracing on **Gemma-2-2B** using Cross-Layer Transcoders (**CLT-HP**) on Neuronpedia: 

* **Baseline (v1):** neurotraceraineu-1794824987766 (2,104 nodes / 51,042 links)
* **Normalized (v2):** neurotraceraiisa-1794889522299 (2,061 nodes / 44,182 links)
* **Focused (v3):** neurotraceraiisa-1794890072063 (1,311 nodes / 14,313 links — **-71.96% edge reduction**)

#### Citation

If you use this methodology or reference implementation in your research, please cite the preprint on Zenodo: 

bibtex

@article{ivanova2026neurotracer,
  title={Neurotracer AI: A Methodology for Preserving Human Meaning, Verifiable Interpretation, and Safe AI Agent Control in Cross-Lingual Environments},
  author={Ivanova, Anna},
  year={2026},
  publisher={Zenodo},
  doi={10.5281/zenodo.24341954},
  url={https://doi.org/10.5281/zenodo.24341954}
}

Используйте код с осторожностью.

Скопировать код в буфер обмена.
