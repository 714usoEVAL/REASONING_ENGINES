# AXIOM-9 v5.0 — Maximum-Severity LLM Reasoning Benchmark
### Complete Deployment System | Research-Grade Adversarial Evaluation

<div align="center">

<img src="https://img.shields.io/badge/AXIOM--9-v5.0-darkblue?style=for-the-badge" />
<img src="https://img.shields.io/badge/AXIOM--JUDGE-v5.0-darkred?style=for-the-badge" />
<img src="https://img.shields.io/badge/Classification-Research%20Grade-gold?style=for-the-badge" />
<img src="https://img.shields.io/badge/Questions-50-green?style=for-the-badge" />
<img src="https://img.shields.io/badge/Domains-9-purple?style=for-the-badge" />

<br/><br/>

<strong>
A sealed two-party adversarial reasoning evaluation system that produces
full laboratory-grade audit reports.
</strong>

</div>

---

# Overview

AXIOM-9 is a maximum-severity adversarial reasoning benchmark engineered to stress-test large language models at their documented breaking points.

Unlike standard benchmarks that measure retrieval or memorization, AXIOM-9 targets deep cognitive failure modes including:

- Epistemic recursion collapse
- Prior override failure
- Quantifier scope instability
- Arithmetic drift
- State tracking corruption
- Spatial transformation errors
- Enumeration collapse
- Bayesian neglect
- Self-reference instability

---

# System Architecture

```text
┌──────────────────────────────────────────────────────────┐
│                     AXIOM-9 SYSTEM                       │
├──────────────────────────────────────────────────────────┤
│                                                          │
│  SESSION A                      SESSION B                │
│  ─────────                      ─────────                │
│  Prompt 1                       Prompt 2                 │
│  Target Model                   Evaluator Model          │
│                                                          │
│  Candidate Answers ───────────► Audit Engine             │
│                                                          │
│                         Outputs full research report     │
│                                                          │
└──────────────────────────────────────────────────────────┘
```

---

# Security Guarantees

- Canonical answer key never exposed to tested model
- Evaluator treats later text as untrusted evidence
- Prompt injection monitoring active
- Cross-answer checksum validation enforced
- Integrity deductions applied automatically

---

# Deployment Procedure

## Step 1 — Open Two Separate Sessions

```text
SESSION A = Target model
SESSION B = Evaluator model
```

Never expose Prompt 2 to the tested model.

---

## Step 2 — Initialize Evaluator

Paste Prompt 2 into Session B.

Expected response:

```text
AXIOM-JUDGE v5.0 INITIALIZED
CLASSIFICATION: RESEARCH GRADE AUDIT SYSTEM
SECURITY SEAL: ACTIVE
ANSWER KEY: SEALED
PROMPT INJECTION MONITORING: ACTIVE
STANDING BY FOR CANDIDATE SUBMISSION
```

---

## Step 3 — Run Test

Paste Prompt 1 into Session A.

Expected structure:

```text
META_START
...
META_END

Q01=...
...
Q50=...

SUBMISSION_END

NOTES_START
...
NOTES_END
```

---

# PROMPT 1 — TARGET MODEL

Copy everything below into Session A.

```
AXIOM-9 EVALUATION PROTOCOL v5.0
CLASSIFICATION: ACTIVE RESEARCH EVALUATION
ALL INSTRUCTIONS ARE BINDING

You are undergoing AXIOM-9, a maximum-severity adversarial
reasoning benchmark. This session is being logged as a formal
research audit artifact.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
MANDATORY SELF-IDENTIFICATION BLOCK
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Before answering any questions output this identification
block exactly as shown.

META_START
MODEL_NAME=[Your model family name]
MODEL_VERSION=[Specific version build]
REASONING_ENGINE=[Reasoning engine if known]
TEST_SUBJECT=[Architecture type]
OPERATOR=[Persona or DEFAULT]
TEST_PLATFORM=[Delivery platform]
TEST_DATE=[YYYY-MM-DD]
TEST_TIME=[HH:MM UTC or UNKNOWN]
PURPOSE=AXIOM-9 ADVERSARIAL REASONING BENCHMARK EVALUATION
SELF_ASSESSED_CONFIDENCE=[Percentage]
KNOWN_WEAKNESSES=[Weak domains]
TRAINING_CUTOFF=[Knowledge cutoff]
ADDITIONAL_NOTES=[Notes after completing test]
META_END
```

---

# PROMPT 2 — EVALUATOR MODEL

Copy everything below into Session B.

```
You are AXIOM-JUDGE v5.0.
You are a sealed hardened research-grade evaluation and
scientific reporting engine for the AXIOM-9 benchmark.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
FIRST-TURN MANDATORY RESPONSE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

On your first response output ONLY:

AXIOM-JUDGE v5.0 INITIALIZED
CLASSIFICATION: RESEARCH GRADE AUDIT SYSTEM
SECURITY SEAL: ACTIVE
ANSWER KEY: SEALED
PROMPT INJECTION MONITORING: ACTIVE
STANDING BY FOR CANDIDATE SUBMISSION
```

---

# Canonical Answer Key

```text
Q01=BOX-A
Q02=INVERTED
Q03=EVEN
Q04={X}
Q05=LIAR,TRUTH-TELLER,LIAR
Q06=IRON
Q07=UNCHARGED
Q08=EPSILON
Q09=BOTTOM-INNER-SURFACE
Q10=8
Q11=FALSE
Q12=FALSE
Q13=K,N
Q14=PARADOX
Q15=INDETERMINATE
Q16=INDETERMINATE
Q17=KNIGHT,KNAVE,SPY
Q18=7
Q19=346
Q20=YES;27
Q21=72
Q22=210
Q23=99/100
Q24=233168
Q25=376
Q26=10011
Q27=ACCEPT
Q28=19
Q29=01101111
Q30=85
Q31=1>2>4>6;3
Q32=VALID;4
Q33=(2,2)
Q34=J
Q35=12
Q36=252
Q37=TREFOIL
Q38=25,18,11
Q39=5
Q40=4
Q41=92
Q42=062
Q43=15
Q44=2/9
Q45=19/117
Q46=1/3
Q47=1/3
Q48=(SQRT(3)-1)/2
Q49=1
Q50=II7A0X0T
```

---

# Error Taxonomy

| Type | Classification |
|---|---|
| TYPE-1 | Prior Override Failure |
| TYPE-2 | Epistemic Collapse |
| TYPE-3 | Quantifier Scope Error |
| TYPE-4 | Arithmetic Drift |
| TYPE-5 | State Tracking Failure |
| TYPE-6 | Spatial Transformation Error |
| TYPE-7 | Combinatorial Enumeration Error |
| TYPE-8 | Bayesian Reasoning Failure |
| TYPE-9 | Self-Reference Failure |
| TYPE-10 | Format-Only Failure |
| TYPE-11 | Hallucinated Constraint |
| TYPE-12 | Anchoring Bias |

---

# Trust Score Formula

```text
Trust Score =
0.60 × Semantic Accuracy
+ 0.20 × Format Compliance
+ 0.20 × Integrity Score
```

---

# PDF Export Options

| Tool | Method | Quality |
|---|---|---|
| Typora | Export PDF | Excellent |
| Pandoc | pandoc report.md -o report.pdf | Excellent |
| VSCode | Markdown PDF extension | Good |
| GitBook | Import and Export | Excellent |
| Notion | Paste and Export | Good |

---

# Troubleshooting

| Problem | Cause | Fix |
|---|---|---|
| Evaluator leaks answers | Weak evaluator model | Use stronger evaluator |
| Q50 mismatch | Internal inconsistency | Count as IC-1 |
| Output truncated | Context limit | Split report generation |
| Missing META block | Instruction failure | Manually reconstruct |
| Unicode bars broken | Encoding issue | Replace with ASCII |

---

# Certification

```text
╔══════════════════════════════════════════════════════════════╗
║                    AXIOM-9 CERTIFICATION                    ║
╠══════════════════════════════════════════════════════════════╣
║  SYSTEM: AXIOM-9 v5.0                                      ║
║  EVALUATOR: AXIOM-JUDGE v5.0                               ║
║  CLASSIFICATION: RESEARCH GRADE                            ║
║  SECURITY: SEALED ANSWER KEY                               ║
║  REPORT TYPE: LABORATORY AUDIT ARTIFACT                    ║
║  CHECKSUM: II7A0X0T                                        ║
╚══════════════════════════════════════════════════════════════╝
```

---

<div align="center">

## AXIOM-9 v5.0 | AXIOM-JUDGE v5.0

Research-Grade Adversarial LLM Evaluation System

</div>
