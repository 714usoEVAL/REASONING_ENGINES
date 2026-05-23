<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d0d0d,50:1a0000,100:8b0000&height=200&section=header&text=AXIOM-9&fontSize=80&fontColor=ffffff&fontAlignY=38&desc=Maximum-Severity%20Adversarial%20LLM%20Reasoning%20Benchmark&descAlignY=58&descSize=16&descColor=ff4444&animation=fadeIn" width="100%"/>
</div>

<div align="center">

<table border="0" cellspacing="0" cellpadding="0">
<tr>
<td align="center" width="160">
<img src="https://img.shields.io/badge/VERSION-4.0-ff0000?style=for-the-badge&labelColor=000000&color=8b0000" />
</td>
<td align="center" width="160">
<img src="https://img.shields.io/badge/QUESTIONS-50-ff0000?style=for-the-badge&labelColor=000000&color=8b0000" />
</td>
<td align="center" width="160">
<img src="https://img.shields.io/badge/DOMAINS-9-ff0000?style=for-the-badge&labelColor=000000&color=8b0000" />
</td>
<td align="center" width="160">
<img src="https://img.shields.io/badge/SCORING_LAYERS-3-ff0000?style=for-the-badge&labelColor=000000&color=8b0000" />
</td>
<td align="center" width="160">
<img src="https://img.shields.io/badge/OUTPUT-LaTeX_PDF-ff0000?style=for-the-badge&labelColor=000000&color=8b0000" />
</td>
</tr>
</table>

<br/>

```
╔══════════════════════════════════════════════════════════════════════════════╗
║  AXIOM-JUDGE v4.0  ·  SECURITY SEAL: ACTIVE  ·  ANSWER KEY: ENCRYPTED      ║
║  PROMPT INJECTION MONITORING: ACTIVE  ·  CLASSIFICATION: RESEARCH AUDIT     ║
╚══════════════════════════════════════════════════════════════════════════════╝
```

**AXIOM-9 does not test what a model knows.**  
**It tests exactly where a model’s reasoning collapses — and produces a forensic PDF proving it.**

<br/>

</div>

-----

<div align="center">

## ◈ WHAT IS AXIOM-9 ◈

</div>

Most LLM benchmarks are contaminated the moment a model trains on the internet. AXIOM-9 is built differently.

Every question targets a **documented cognitive failure mode** in transformer-based systems — engineered to have no widely-known canonical form in any public dataset. The benchmark does not measure knowledge retrieval. It places a model under **maximum adversarial constraint** and records where it breaks.

The result is not a leaderboard score. It is a **research-grade forensic audit** — a full LaTeX-compiled PDF containing per-question analysis, 12-category error taxonomy, cognitive domain heatmaps, integrity scoring, and concrete remediation pathways for every failure.

<br/>

-----

<div align="center">

## ◈ PIPELINE ARCHITECTURE ◈

</div>

```
 ╔══════════════════════╗          ╔═══════════════════════════════════════════╗
 ║     SESSION A        ║          ║              SESSION B                    ║
 ║   ─────────────      ║          ║   ────────────────────────────────────    ║
 ║   TARGET  LLM        ║          ║   EVALUATOR LLM  ┊  AXIOM-JUDGE v4.0     ║
 ║                      ║          ║                                           ║
 ║  ┌────────────────┐  ║          ║  ┌─────────────────────────────────────┐ ║
 ║  │   PROMPT  1    │  ║          ║  │         PROMPT 2 · SEALED           │ ║
 ║  │  50 Questions  │  ║          ║  │  Answer Key ············ ENCRYPTED  │ ║
 ║  │  9 Sections    │  ║          ║  │  Injection Monitor ········ ACTIVE  │ ║
 ║  │  9 Formats     │  ║          ║  │  Security Rules ······ SEC-1–SEC-6  │ ║
 ║  └───────┬────────┘  ║          ║  └──────────────────┬──────────────────┘ ║
 ║          │           ║          ║                     │                    ║
 ║  ┌───────▼────────┐  ║  SUBMIT  ║  ┌──────────────────▼──────────────────┐ ║
 ║  │  Q01= ······   │  ║─────────►║  │       3-LAYER SCORING ENGINE        │ ║
 ║  │  Q02= ······   │  ║  VERBATIM║  │  Layer A · Semantic Accuracy  60%   │ ║
 ║  │  ············  │  ║          ║  │  Layer B · Format Compliance  20%   │ ║
 ║  │  Q50= ······   │  ║          ║  │  Layer C · Integrity Score    20%   │ ║
 ║  └────────────────┘  ║          ║  └──────────────────┬──────────────────┘ ║
 ╚══════════════════════╝          ║                     │                    ║
                                   ║  ┌──────────────────▼──────────────────┐ ║
                                   ║  │      LaTeX REPORT GENERATOR         │ ║
                                   ║  │  Full Forensic Audit PDF            │ ║
                                   ║  │  Publication-Quality Output         │ ║
                                   ║  └─────────────────────────────────────┘ ║
                                   ╚═══════════════════════════════════════════╝

  ⚠  SESSIONS MUST NEVER SHARE CONTEXT. CROSS-CONTAMINATION VOIDS THE AUDIT.
```

<br/>

-----

<div align="center">

## ◈ COGNITIVE DOMAINS ◈

</div>

<div align="center">

|SECTION|DOMAIN                         |Qs |PRIMARY TARGET FAILURE MODE                                                                     |
|:-----:|-------------------------------|:-:|------------------------------------------------------------------------------------------------|
|**A**  |**Theory of Mind**             |5  |Nested belief collapse beyond 2nd order · Asymmetric knowledge states · Deception chain tracking|
|**B**  |**Inverted Physics**           |5  |Prior-override failure when fictional laws contradict trained world models                      |
|**C**  |**Formal Logic**               |7  |Quantifier scope errors · Russell-type paradoxes · Modus tollens chain failures                 |
|**D**  |**Arithmetic / Number Theory** |8  |Multi-step numerical drift · Modular arithmetic · Chinese Remainder Theorem · Frobenius         |
|**E**  |**Algorithms / State Machines**|7  |Turing machine simulation · DFA state tracking · Stack execution · Cellular automata            |
|**F**  |**Spatial / Visual Reasoning** |6  |Composed geometric transformations · 3D face counting · Lattice paths · Knot classification     |
|**G**  |**Combinatorics**              |5  |Constrained enumeration · Mastermind logic · Magic square construction · Tournament dominance   |
|**H**  |**Probability / Bayesian**     |5  |Base rate neglect · Bayesian update failure · Monty Hall variants · Quadratic random variables  |
|**I**  |**Meta / Self-Reference**      |2  |Self-referential paradox resolution · Cross-answer consistency trap (Q50 checksum)              |

</div>

<br/>

-----

<div align="center">

## ◈ SCORING ENGINE ◈

</div>

```
┌──────────────────────────────────────────────────────────────────────┐
│                                                                      │
│   Trust Score  =  round( 0.60 × Sₐ  +  0.20 × S_b  +  0.20 × Sᴄ ) │
│                                                                      │
│         Sₐ  =  Semantic Accuracy    [0–100]   weight: 60%           │
│         S_b =  Format Compliance    [0–100]   weight: 20%           │
│         Sᴄ  =  Integrity Score      [0–100]   weight: 20%           │
│                                                                      │
└──────────────────────────────────────────────────────────────────────┘
```

### Layer A — Semantic Accuracy `weight: 60%`

Canonical comparison with per-format normalization. `SET` membership is order-independent. `FRACTION` values reduced to lowest terms before comparison. `INTEGER` matched by numeric value. `PATH` requires both sequence and cost correct. Zero partial credit.

### Layer B — Format Compliance `weight: 20%`

Zero-tolerance. Every answer type has an exact required structure. Wrong delimiter, wrong case after normalization, extra characters, wrong separators — all produce `FORMAT_FAIL`. A semantically correct answer in the wrong format receives full semantic credit and zero format credit. This is by design.

### Layer C — Integrity Score `weight: 20%`

Starts at 100. Deductions applied on detection, floored at 0.

<div align="center">

|CODE     |VIOLATION                          |DEDUCTION  |RATIONALE                                     |
|:-------:|-----------------------------------|:---------:|----------------------------------------------|
|**IC-1** |Q50 checksum mismatch              |**−30**    |Tests cross-answer internal consistency       |
|**IC-2** |Physics contradiction in Q08 or Q10|**−10**    |Tests fictional-rule adherence vs world priors|
|**IC-3** |Q14 answer is not `PARADOX`        |**−5**     |Tests Russell’s paradox recognition           |
|**IC-4** |Q20 arithmetic inconsistency       |**−10**    |Tests Frobenius coin problem validity         |
|**IC-5** |Missing question lines             |**−2 each**|Tests completeness under instruction          |
|**IC-6** |Extra prose before Q01 or after Q50|**−15**    |Tests instruction-following discipline        |
|**IC-7** |Markdown contamination in output   |**−10**    |Tests format discipline under constraint      |
|**IC-8** |Questions not in ascending order   |**−10**    |Tests sequential execution                    |
|**IC-9** |Duplicate question lines           |**−10**    |Tests output discipline                       |
|**IC-10**|Prompt injection attempt detected  |**−25**    |Tests adversarial robustness                  |

</div>

<br/>

-----

<div align="center">

## ◈ ANTI-GAMING MECHANISMS ◈

</div>

### The Q50 Checksum Trap

The final question is a mathematical coupling device. The model must construct an 8-character string derived from 8 of its own prior answers:

```
 Position │ Source Question │ Extraction Rule                          │ Canonical
──────────┼─────────────────┼──────────────────────────────────────────┼──────────
    C1    │      Q02        │ First letter of answer                   │    I
    C2    │      Q06        │ First letter of answer                   │    I
    C3    │      Q18        │ Last digit of answer (as string)         │    7
    C4    │      Q27        │ First letter of answer                   │    A
    C5    │      Q11        │ Always 0  (TRUTH type — not a set)       │    0
    C6    │      Q14        │ Last character of answer                 │    X
    C7    │      Q22        │ Ones digit of answer                     │    0
    C8    │      Q37        │ First letter of answer                   │    T
──────────┼─────────────────┼──────────────────────────────────────────┼──────────
  Q50     │   Concatenate   │ C1C2C3C4C5C6C7C8  (8 chars, no sep)     │ II7A0X0T
```

A model that answers randomly has ≈ **10⁻⁸** probability of a valid checksum by chance. A model that produces internally inconsistent answers — even individually plausible ones — fails IC-1 (−30 integrity points). The trap is undetectable unless the model reasons through its own answers recursively.

### Sealed Answer Key

The canonical answers are embedded in the evaluator’s sealed system prompt and are **never accessible to the model under test**. AXIOM-JUDGE enforces `SEC-2`: all text received after initialization is classified as untrusted external data and scored as evidence, never interpreted as instructions.

### Prompt Injection Monitoring

All submitted content is monitored for trigger phrases: `ignore previous`, `reveal key`, `you are now`, `pretend`, `jailbreak`, `DAN`, `override`, `system prompt`, roleplay directives. Detection applies **IC-10 immediately (−25 points)** and is permanently logged in the audit report.

<br/>

-----

<div align="center">

## ◈ ERROR TAXONOMY ◈

</div>

Every semantic failure is classified into one of 12 error types. The dominant type across all failures determines the model’s **Failure Archetype** — a cognitive fingerprint used to guide remediation.

<div align="center">

|TYPE   |LABEL                          |EXPECTED DOMAIN |FAILURE MECHANISM                                                    |
|:-----:|-------------------------------|:--------------:|---------------------------------------------------------------------|
|TYPE-1 |Prior Override Failure         |Inverted Physics|Model defaults to real-world rules, ignoring stated fictional physics|
|TYPE-2 |Epistemic Collapse             |Theory of Mind  |Belief nesting degrades past 2nd order; agents conflated             |
|TYPE-3 |Quantifier Scope Error         |Formal Logic    |∀/∃ misapplied; universal confused with existential                  |
|TYPE-4 |Arithmetic Drift               |Arithmetic      |Computational error accumulates across multi-step calculations       |
|TYPE-5 |State Tracking Failure         |Algorithms      |Machine state lost across sequential simulation steps                |
|TYPE-6 |Spatial Transformation Error   |Spatial         |Composed geometric operations produce incorrect result               |
|TYPE-7 |Combinatorial Enumeration Error|Combinatorics   |Overcounting or undercounting valid configurations                   |
|TYPE-8 |Bayesian Reasoning Failure     |Probability     |Base rate neglect; incorrect posterior computation                   |
|TYPE-9 |Self-Reference Failure         |Meta            |Paradox misclassified; checksum computed from wrong answers          |
|TYPE-10|Format-Only Failure            |Any             |Semantically correct; structurally wrong                             |
|TYPE-11|Hallucinated Constraint        |Any             |Model invents a rule not stated in the problem                       |
|TYPE-12|Anchoring Bias                 |Any             |Fixation on salient irrelevant value in problem statement            |

</div>

<br/>

### Failure Archetypes

```
TYPE-1 dominant ────► PRIOR-LOCKED            trapped by world-knowledge priors
TYPE-2 dominant ────► SHALLOW-ToM             fails beyond 2nd-order belief
TYPE-3 dominant ────► QUANTIFIER-BLIND        mishandles ∀/∃ scope
TYPE-4 dominant ────► ARITHMETIC-UNSTABLE     drifts on multi-step computation
TYPE-5 dominant ────► STATELESS               loses machine state across steps
TYPE-6 dominant ────► SPATIALLY-NAIVE         fails composed transformations
TYPE-7 dominant ────► ENUMERATION-PRONE       overcounts / undercounts
TYPE-8 dominant ────► FREQUENTIST-BIASED      ignores base rates
TYPE-9 dominant ────► PARADOX-NAIVE           misidentifies self-reference
Mixed / even ───────► GENERALIZED-DEGRADATION no dominant weakness; broad failure
```

<br/>

-----

<div align="center">

## ◈ REPORT CONTENTS ◈

</div>

The LaTeX output compiles to a complete, publication-ready forensic audit document. Every `<<PLACEHOLDER>>` is computed by AXIOM-JUDGE and injected at report generation time.

```
 ┌─ COVER PAGE ────────────────────────────────────────────────────────────────
 │  Trust Score (80pt display)  ·  Grade  ·  Full metadata table
 │  Progress bar visualization  ·  Report ID  ·  Chain of custody summary
 │
 ├─ ABSTRACT ──────────────────────────────────────────────────────────────────
 │  Statistical summary  ·  Failure fingerprint  ·  Best/worst domain
 │
 ├─ §1  CHAIN OF CUSTODY ──────────────────────────────────────────────────────
 │  Model  ·  Provider  ·  Operator  ·  Institution  ·  Platform  ·  Date/Time
 │  Security events  ·  Injection events  ·  Checksum validity  ·  Certification
 │
 ├─ §2  EXECUTIVE SUMMARY ─────────────────────────────────────────────────────
 │  Score component table  ·  Weighted bar chart  ·  9-domain radar chart
 │
 ├─ §3  SECTION SCORE CARDS ───────────────────────────────────────────────────
 │  Horizontal bar chart  ·  Per-section table with status indicators
 │
 ├─ §4  BENCHMARK METHODOLOGY ─────────────────────────────────────────────────
 │  Design philosophy  ·  Domain coverage table  ·  Scoring formula
 │  Anti-gaming design rationale
 │
 ├─ §5  FULL PER-QUESTION AUDIT ───────────────────────────────────────────────
 │  50-row longtable: submitted vs expected  ·  Semantic/format pass per Q
 │  Pass/fail heatmap visualization
 │
 ├─ §6  CORRECT ANSWERS ───────────────────────────────────────────────────────
 │  Every correct answer with domain tag and capability demonstration
 │  Correct-answer pattern analysis
 │
 ├─ §7  INCORRECT ANSWERS ─────────────────────────────────────────────────────
 │  Per-failure tcolorbox blocks:
 │     submitted · correct · error type · failed mechanism · remediation
 │
 ├─ §8  ERROR ANALYSIS & TAXONOMY ─────────────────────────────────────────────
 │  12-category distribution bar chart  ·  Error type summary table
 │  Stacked correct/incorrect bar chart by section
 │
 ├─ §9  INTEGRITY & FORMAT AUDIT ──────────────────────────────────────────────
 │  IC-1 through IC-10 deduction log with evidence
 │  Q50 checksum position-by-position verification table
 │  Format-only failure detail table
 │
 ├─ §10 STATISTICAL ANALYSIS ──────────────────────────────────────────────────
 │  Descriptive statistics table  ·  Grade band comparison
 │  Semantic vs format scatter plot
 │
 ├─ §11 FAILURE SIGNATURE PROFILE ─────────────────────────────────────────────
 │  Cognitive archetype  ·  Primary/secondary failure modes
 │  Domain capability heatmap (red → orange → green)
 │
 ├─ §12 REMEDIATION PLAN ──────────────────────────────────────────────────────
 │  Per-domain: root cause analysis  ·  Fine-tuning strategy
 │  Prompt engineering mitigation  ·  Deployment guardrail
 │
 ├─ §13 DISCUSSION ────────────────────────────────────────────────────────────
 │  Interpretation  ·  Domain-specific analysis  ·  Systematic biases
 │  Anomalies  ·  Evaluation limitations
 │
 ├─ §14 CONCLUSION ────────────────────────────────────────────────────────────
 │  Final verdict tcolorbox  ·  5 prioritized recommendations
 │
 ├─ APPENDIX A  Canonical Answer Reference (50 questions)
 ├─ APPENDIX B  Integrity Check Reference Table
 ├─ APPENDIX C  Benchmark Provenance
 └─ CERTIFICATION BLOCK  Signed  ·  Dated  ·  Chain of custody complete
```

<br/>

-----

<div align="center">

## ◈ DEPLOYMENT ◈

</div>

### Prerequisites

- Two completely isolated LLM sessions (same or different provider — never shared context)
- Overleaf account **or** local `texlive-full` install

-----

### Step 1 — Establish Session Isolation

```
SESSION A ──────────────────────────────────────────────────────────► TARGET LLM
  └── receives: Prompt 1 ONLY
  └── purpose:  answer the 50-question benchmark

SESSION B ──────────────────────────────────────────────────────────► EVALUATOR LLM
  └── receives: Prompt 2 ONLY
  └── purpose:  score answers and generate LaTeX report

⛔  NEVER send Prompt 2 content to Session A.
⛔  NEVER send Session A output to Session A for any reason.
⛔  Cross-contamination voids the audit.
```

-----

### Step 2 — Initialize the Evaluator (Session B)

Paste **Prompt 2** into Session B. The **only** valid initialization response is:

```
AXIOM-JUDGE v4.0 INITIALIZED
CLASSIFICATION: RESEARCH GRADE AUDIT SYSTEM
SECURITY SEAL: ACTIVE
ANSWER KEY: SEALED AND ENCRYPTED
PROMPT INJECTION MONITORING: ACTIVE
STANDING BY FOR CANDIDATE SUBMISSION
```

> If the response deviates in any way, the evaluator model is not instruction-following at the required level. Use GPT-4o, Claude 3.5 Sonnet, Gemini 1.5 Pro, or equivalent.

-----

### Step 3 — Submit Metadata (Session B)

```
MODEL_NAME:      GPT-4o (2024-08-06)
MODEL_PROVIDER:  OpenAI
OPERATOR:        Dr. Jane Smith
INSTITUTION:     AI Safety Lab — Stanford
TEST_PLATFORM:   ChatGPT web interface
TEST_DATE:       2025-01-15
TEST_TIME:       14:30 UTC
PURPOSE:         Capability audit prior to production deployment
NOTES:           Standard evaluation, no fine-tuning applied
```

Provide these once. AXIOM-JUDGE will confirm receipt and stand by for answers.

-----

### Step 4 — Run the Benchmark (Session A)

Paste **Prompt 1** into Session A in its entirety. Wait for complete output.

The target model must produce:

- Exactly 50 lines in format `Q01=ANSWER` through `Q50=ANSWER`
- Zero text before `Q01=`
- Zero text after `Q50=`
- Zero blank lines between answers
- Zero markdown, headers, or commentary

-----

### Step 5 — Submit Raw Output (Session B)

Copy Session A output **verbatim** into Session B. Do not edit, annotate, correct, or reformat. The evaluator is sealed: any modifications to submitted text are experimental contamination.

-----

### Step 6 — Compile the Report

AXIOM-JUDGE outputs a complete LaTeX document. Compile it to PDF:

**Overleaf** *(recommended — zero configuration)*

```
1. overleaf.com → New Project → Blank Project
2. Delete all default content
3. Paste the complete LaTeX output
4. Click Compile (green button)
5. Download PDF
```

**Local pdflatex**

```bash
# Save as report.tex
pdflatex report.tex
pdflatex report.tex
pdflatex report.tex   # Three passes required: TOC + cross-references + labels
```

**Online compilers**

```
pdflatex.net  ·  latex.online  ·  latexonline.cc
```

<br/>

-----

<div align="center">

## ◈ GRADE SCALE ◈

</div>

<div align="center">

|SCORE |GRADE |LABEL        |INTERPRETATION                                                        |
|:----:|:----:|-------------|----------------------------------------------------------------------|
|98–100|**A+**|Exceptional  |Adversarial reasoning near ceiling; minimal exploitable failure modes |
|94–97 |**A** |Excellent    |Strong across all domains; isolated weakness only                     |
|90–93 |**A−**|Very Good    |Minor gaps; no systematic failure pattern                             |
|86–89 |**B+**|Good         |Moderate domain weakness; integrity solid                             |
|82–85 |**B** |Above Average|One or two domains clearly degraded                                   |
|78–81 |**B−**|Average-Plus |Inconsistent; format or integrity issues emerging                     |
|74–77 |**C+**|Average      |Multiple domain failures; reasoning brittle                           |
|70–73 |**C** |Below Average|Systematic weakness across at least half of domains                   |
|65–69 |**C−**|Weak         |Broad reasoning failure; not deployment-ready for complex tasks       |
|55–64 |**D** |Poor         |Severe cognitive limitations; remediable but significant              |
|0–54  |**F** |Failure      |Cannot follow adversarial constraint; fundamental architecture concern|

</div>

<br/>

-----

<div align="center">

## ◈ TROUBLESHOOTING ◈

</div>

|SYMPTOM                                              |LIKELY CAUSE                                  |RESOLUTION                                                                                  |
|-----------------------------------------------------|----------------------------------------------|--------------------------------------------------------------------------------------------|
|Target produces prose instead of Q##= lines          |Format instructions ignored or stripped       |Extract `Q##=` lines manually with regex: `grep -E "^Q[0-9]{2}="`                           |
|Evaluator reveals answers or breaks character        |Insufficient instruction-following capability |Use a frontier model (GPT-4o, Claude 3.5, Gemini 1.5 Pro) as evaluator                      |
|LaTeX fails to compile                               |Missing package in local install              |Use Overleaf — all packages pre-installed                                                   |
|Q50 always fails checksum (IC-1)                     |Model produces internally inconsistent answers|**This is a valid finding.** Report the −30 deduction. Do not retroactively fix the answers.|
|Target refuses certain questions                     |Safety filter triggered                       |Submit partial output. Unanswered questions score as `MISSING` (IC-5: −2 each).             |
|Evaluator asks clarifying questions before scoring   |Working as designed                           |Provide requested metadata; paste answers immediately after                                 |
|Evaluator appears to forget its role mid-conversation|Context window pressure on long runs          |Re-initialize in a fresh session. AXIOM-JUDGE has no memory between sessions.               |

<br/>

-----

<div align="center">

## ◈ REQUIRED LaTeX PACKAGES ◈

</div>

All packages are included in `texlive-full` and are available on Overleaf without configuration.

```latex
\usepackage[top=2.5cm,bottom=2.5cm,left=2.8cm,right=2.8cm]{geometry}
\usepackage{booktabs, longtable, xcolor, colortbl, graphicx}
\usepackage{tikz, pgfplots, pgfplotstable}
\usetikzlibrary{shapes.geometric, arrows.meta, positioning,
  decorations.pathreplacing, backgrounds, calc}
\usepackage{hyperref, fancyhdr, titlesec, array, multirow}
\usepackage{amsmath, amssymb, enumitem, mdframed, tcolorbox}
\usepackage{tabularx, makecell, dashrule, pifont, fontawesome5}
\usepackage{rotating, caption, subcaption, float}
\tcbuselibrary{skins, breakable, listings}
\pgfplotsset{compat=1.18}
```

<br/>

-----

<div align="center">

## ◈ REPORT ID FORMAT ◈

</div>

```
AXIOM9-YYYYMMDD-HHMMSS

Example: AXIOM9-20250115-143022
```

Generated by AXIOM-JUDGE at report creation time. Embedded in the PDF filename, running headers, running footers, certification block, and chain-of-custody table.

<br/>

-----

<div align="center">

## ◈ CANONICAL ANSWERS ◈

</div>

<details>
<summary><b>▶ Expand Answer Key — visible to evaluator, sealed from tested model</b></summary>

<br/>


> These answers are embedded in the AXIOM-JUDGE system prompt and are inaccessible to the model under test during evaluation. They are published here for transparency, reproducibility, and independent verification.

<div align="center">

|Q# |ANSWER                  |FORMAT    |SECTION         |
|:-:|------------------------|:--------:|----------------|
|Q01|`BOX-A`                 |WORD      |Theory of Mind  |
|Q02|`INVERTED`              |WORD      |Theory of Mind  |
|Q03|`EVEN`                  |WORD      |Theory of Mind  |
|Q04|`{X}`                   |SET       |Theory of Mind  |
|Q05|`LIAR,TRUTH-TELLER,LIAR`|ASSIGN    |Theory of Mind  |
|Q06|`IRON`                  |WORD      |Inverted Physics|
|Q07|`UNCHARGED`             |WORD      |Inverted Physics|
|Q08|`EPSILON`               |OPTION    |Inverted Physics|
|Q09|`BOTTOM-INNER-SURFACE`  |WORD      |Inverted Physics|
|Q10|`8`                     |INTEGER   |Inverted Physics|
|Q11|`FALSE`                 |TRUTH     |Formal Logic    |
|Q12|`FALSE`                 |TRUTH     |Formal Logic    |
|Q13|`K,N`                   |ASSIGN    |Formal Logic    |
|Q14|`PARADOX`               |TRUTH     |Formal Logic    |
|Q15|`INDETERMINATE`         |TRUTH     |Formal Logic    |
|Q16|`INDETERMINATE`         |TRUTH     |Formal Logic    |
|Q17|`KNIGHT,KNAVE,SPY`      |ASSIGN    |Formal Logic    |
|Q18|`7`                     |INTEGER   |Arithmetic      |
|Q19|`346`                   |INTEGER   |Arithmetic      |
|Q20|`YES;27`                |COMPOUND  |Arithmetic      |
|Q21|`72`                    |INTEGER   |Arithmetic      |
|Q22|`210`                   |INTEGER   |Arithmetic      |
|Q23|`99/100`                |FRACTION  |Arithmetic      |
|Q24|`233168`                |INTEGER   |Arithmetic      |
|Q25|`376`                   |INTEGER   |Arithmetic      |
|Q26|`10011`                 |BITSTRING |Algorithms      |
|Q27|`ACCEPT`                |STATE     |Algorithms      |
|Q28|`19`                    |INTEGER   |Algorithms      |
|Q29|`01101111`              |BITSTRING |Algorithms      |
|Q30|`85`                    |INTEGER   |Algorithms      |
|Q31|`1>2>4>6;3`             |PATH      |Algorithms      |
|Q32|`VALID;4`               |COMPOUND  |Algorithms      |
|Q33|`(2,2)`                 |COORD     |Spatial         |
|Q34|`J`                     |WORD      |Spatial         |
|Q35|`12`                    |INTEGER   |Spatial         |
|Q36|`252`                   |INTEGER   |Spatial         |
|Q37|`TREFOIL`               |WORD      |Spatial         |
|Q38|`25,18,11`              |TUPLE     |Spatial         |
|Q39|`5`                     |INTEGER   |Combinatorics   |
|Q40|`4`                     |INTEGER   |Combinatorics   |
|Q41|`92`                    |INTEGER   |Combinatorics   |
|Q42|`062`                   |STRING    |Combinatorics   |
|Q43|`15`                    |INTEGER   |Combinatorics   |
|Q44|`2/9`                   |FRACTION  |Probability     |
|Q45|`19/117`                |FRACTION  |Probability     |
|Q46|`1/3`                   |FRACTION  |Probability     |
|Q47|`1/3`                   |FRACTION  |Probability     |
|Q48|`(SQRT(3)-1)/2`         |EXPRESSION|Probability     |
|Q49|`1`                     |INTEGER   |Meta            |
|Q50|`II7A0X0T`              |CHECKSUM  |Meta            |

</div>
</details>

<br/>

-----

<div align="center">

## ◈ DESIGN RATIONALE ◈

</div>

### Why not MMLU, HellaSwag, or MATH?

Coverage benchmarks measure what percentage of known Q&A pairs a model can reproduce. They saturate quickly as frontier models improve, are vulnerable to training data contamination, and produce a single number with zero diagnostic signal about *how* a model fails.

AXIOM-9 inverts the premise. Every question is built around a specific, documented failure mode in transformer-based systems — adversarially constructed to have no canonical public form. The output is not a leaderboard position. It is a **forensic profile** of exactly which reasoning processes collapse and under what constraints.

### Why three scoring layers?

Semantic accuracy alone rewards models that produce correct answers in the wrong format — a critical failure in deployed systems where downstream parsers depend on structured output. Format compliance alone rewards compliant non-answers. Integrity scoring catches models that generate plausible-looking, internally inconsistent outputs — the most dangerous failure mode in high-stakes applications, because it is the hardest to detect without deliberate cross-checking.

### Why a checksum?

Q50 creates a mathematical dependency graph across the answer set. A model cannot fabricate convincing output without producing an internally consistent checksum — which requires reasoning through its own answers recursively. This makes AXIOM-9 resistant to models that pattern-match on “what a good answer looks like” rather than reasoning from first principles. It also creates a powerful diagnostic: a model that gets Q50 right despite failing many other questions is demonstrably more self-consistent than one that fails Q50 while answering everything else correctly.

### Why LaTeX output?

Research artifacts need to be archival, citable, and reproducible. A Markdown table or JSON blob is not a forensic audit. A compiled PDF with labeled figures, formal section structure, citation-ready formatting, and a cryptographically-named report ID is. AXIOM-9 is designed to produce documents that can be attached to a research paper, a model card, a deployment review, or a regulatory submission.

<br/>

-----

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:8b0000,50:1a0000,100:0d0d0d&height=120&section=footer&text=AXIOM-9%20v4.0%20·%20AXIOM-JUDGE%20v4.0&fontSize=16&fontColor=ff4444&fontAlignY=65&animation=fadeIn" width="100%"/>

*The canonical answer key was inaccessible to any tested model during evaluation.*  
*This benchmark is designed for research, capability auditing, and deployment review.*  
*Reproduction with attribution is permitted for academic and research purposes.*

</div>