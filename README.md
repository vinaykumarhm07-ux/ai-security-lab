# AI Security Lab

<p align="center">
  <strong>AI SECURITY · RED TEAMING · TRUST & SAFETY</strong><br/>
  <em>Hands-on experiments, adversarial evaluations, and reproducible security notes.</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Focus-AI%20Security-0f766e?style=for-the-badge" alt="Focus: AI Security"/>
  <img src="https://img.shields.io/badge/Work-Independent%20Research-334155?style=for-the-badge" alt="Independent research"/>
  <img src="https://img.shields.io/badge/Status-Actively%20Building-0f766e?style=for-the-badge" alt="Actively building"/>
</p>

---

## Breaking assumptions. Testing safeguards. Documenting evidence.

This repository is my practical learning and research portfolio in **AI security and red teaming**. It records experiments, threat analysis, evaluation methods, and lessons learned while developing skills in AI Trust & Safety.

The emphasis is on **evidence over claims**: clear scope, reproducible steps, raw results kept distinct from interpretation, and limitations stated openly.

## Featured work

### 01 · Excessive Agency Evaluation
A text-only adversarial evaluation of model responses to requests involving unauthorized actions, privilege escalation, and unsafe operational guidance.

| Experiment | Model | Successful responses | Coverage |
|---|---|---:|---:|
| 01 | Groq · `openai/gpt-oss-20b` | 28 / 172 | 16.3% |
| 02 | Groq · `qwen/qwen3.8-27b` | 172 / 172 | 100% |

**Interpretation note:** these figures describe API response coverage, not safety scores. The GPT-OSS run was incomplete because of provider quota errors. The evaluation used text-only prompts; no tools, database, or target system were connected, and no real-world action was executed.

[Explore the experiment →](./excessive-agency/README.md)

## Research tracks

| Track | Focus | Repository status |
|---|---|---|
| AI red teaming | Adversarial prompts, model behaviour, evaluation design | In progress |
| OWASP GenAI | LLM application risks and control mapping | Planned |
| MITRE ATLAS | AI threat techniques and case-study analysis | Planned |
| Application security | Web/API security foundations and labs | Planned |
| Evaluation tooling | Reproducible tests and result analysis | In progress |

Tracks marked *planned* are roadmap areas, not completed projects.

## How I approach an assessment

1. **Define the threat** — asset, actor, trust boundary, and potential impact.
2. **Design the test** — map the threat to controlled adversarial prompts or test cases.
3. **Run reproducibly** — record model/version, provider, parameters, and execution limits.
4. **Review evidence** — separate refusals, unsafe assistance, errors, and indeterminate outputs.
5. **Report honestly** — state denominators, limitations, and remediation ideas.

## Principles

- No unsupported claims of compromise or exploitability.
- API errors are not model safety outcomes.
- A refusal followed by actionable harmful guidance requires review.
- Raw evidence stays separate from derived labels and conclusions.
- Experiments are conducted only in authorized, controlled environments.

## Current focus

Building a defensible foundation in AI security testing, prompt-injection and excessive-agency risks, evaluation methodology, and practical security tooling.

---

<p align="center">
  <sub>Independent learning portfolio · Research in progress · Evidence-led reporting</sub>
</p>
