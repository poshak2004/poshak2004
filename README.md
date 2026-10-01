<div align="center">

# Poshak Kotresha

**AI Product Engineer** · agent systems · governance · automation · ML / CV

<a href="https://github.com/poshak2004"><img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=15&duration=3200&pause=900&color=8B949E&center=true&vCenter=true&width=560&lines=Agents+that+do+real+work+%E2%80%94+safely.;Most+restrictive+decision+wins.;No+model+gets+to+rewrite+its+own+policies.;architecture+%E2%86%92+implementation+%E2%86%92+tests+%E2%86%92+ship" alt="typing" /></a>

<a href="https://linkedin.com/in/poshak-k"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>
<img src="https://img.shields.io/badge/Bengaluru-161b22?style=flat-square&logo=googlemaps&logoColor=white" />
<img src="https://img.shields.io/badge/open_to-AI_Product_%2F_Agent_Engineering-2ea043?style=flat-square" />

</div>

```text
$ whoami
  B.E. Information Science & Engineering, 2026
  Operations Executive @ FAFF (personal AI assistant): I work inside a live
  AI-agent pipeline where tasks go from user to agents to humans and back.

$ cat focus.txt
  I build the layer between "the model said so" and "it actually happened":
  orchestration, deterministic governance, human escalation, evaluation.
```

I spend my days on the operations side of an AI-agent product: research, bookings, calls, vendor coordination, escalations and QA.
My evenings go to the engineering side. Seeing both is why my work is about **control, reliability and humans-in-the-loop**, not just model calls.

---

### ⚙️ The rule I keep building around

```ts
// Every applicable rule votes. The most restrictive decision wins.
const DECISIONS = ['ALLOW', 'RETRY', 'REROUTE', 'WAIT', 'ESCALATE', 'BLOCK'] as const;

// Precedence: safety > system > project > table > role > agent > task
// Lower layers can only tighten. Safety rules can't be waived.
// Policies are loaded from code, never from something the model can edit.
```
<sub>From <a href="https://github.com/poshak2004/pixel-ai-workbench/blob/main/src/core/governance/types.ts"><code>pixel-ai-workbench/src/core/governance</code></a></sub>

---

### 🛠 What I'm building

<table>
<tr>
<td width="50%" valign="top">

#### [**PIXEL**](https://github.com/poshak2004/pixel-ai-workbench) · `TypeScript` `Electron`
A local-first **AI engineering and agent execution environment** for macOS.

`Run → Agent → Role → Model → Provider → Tools → Events → Artifacts → Usage → Eval`

- **Table of Agents:** independent proposals → blind cross-review → rebuttal → adjudication → governance
- Layered **deterministic governance engine** with approvals
- DAG workflows: parallel branches, retries, timeouts, cancellation
- Multi-provider (Anthropic, OpenAI-compatible, Gemini, offline demo), MCP client, sandboxed FS, git worktrees
- Keys in macOS Keychain, redacted event journal, cost accounting
- Vitest + Playwright E2E against the packaged app

</td>
<td width="50%" valign="top">

#### **Governor** · `Python` · _built at work, private_
A **deterministic control plane for AI-agent workflows**. It sits between agent reasoning and execution.

- Decides `ALLOW` / `BLOCK` / `ESCALATE` per task, with clear precedence
- Keeps reasoning and governance separate, and escalates to humans by design
- Learns from outcomes **without** letting a model touch its own code, policy or weights
- **244 tests passing across 6 suites**

#### **Career OS** · `FastAPI` · _in progress_
An autonomous job-intelligence pipeline: discovery → JD analysis → company research → profile matching → application → interview prep → feedback loop.

- `jd_analyzer` and `profile_matcher` modules, with a test suite

</td>
</tr>
</table>

---

### 🧪 Earlier work: where it started

| | Project | What it is |
|---|---|---|
| 📄 | [**industrial-yolo-ocr**](https://github.com/poshak2004/industrial-yolo-ocr) | YOLOv8 layout detection (title / table / text) on **2,676 real industrial invoice PDFs**, built to feed OCR → structured extraction. mAP@50 0.69 |
| 🙂 | [**face-ai-foundations**](https://github.com/poshak2004/face-ai-foundations) | Face detection (Haar, MediaPipe), custom-CNN emotion recognition on FER-2013, MobileNet transfer learning for gender, real-time webcam inference |
| 🌙 | [**luna-soul-guide**](https://github.com/poshak2004/luna-soul-guide) | AI mental-wellness app: chat companion, mood analysis, journaling prompts, weekly summaries via Supabase edge functions + LLM; React/TS |
| 🛡 | [**fraud_detection**](https://github.com/poshak2004/fraud_detection) | Imbalanced-class fraud classification: LR baseline → RF → gradient boosting, recall-first evaluation, ROC + confusion matrix |
| 🧠 | [**Brain-Tumor-Detection**](https://github.com/poshak2004/Brain-Tumor-Detection) | MRI tumor classifier (TensorFlow CNN) served through a Flask web app |
| 🔁 | [**end-to-end-ml-pipeline**](https://github.com/poshak2004/end-to-end-ml-pipeline) | Modular preprocess → train → visualize pipeline with an app entry point |

```text
ML / CV ──▶ AI apps ──▶ full-stack ──▶ agents & automation ──▶ AI systems / product engineering
```

---

### 🧰 Tools I actually use

**Languages:** Python · TypeScript · JavaScript · SQL
**AI / agents:** LLM APIs (Anthropic, OpenAI-compatible, Gemini) · MCP · RAG · agent orchestration · evals · n8n
**ML / CV:** TensorFlow / Keras · scikit-learn · YOLOv8 (Ultralytics) · OpenCV · MediaPipe · OCR · pandas · NumPy
**Backend:** FastAPI · Node.js · Flask · Streamlit · SQLite / Drizzle · Supabase · REST
**Frontend / desktop:** React · Tailwind · Electron
**Shipping:** Git · Docker · pytest · Vitest · Playwright · Power BI

---

<div align="center">
<sub>Currently: making agents more boring, in the good way. Predictable, auditable, and quick to hand off to a human.</sub>
</div>
