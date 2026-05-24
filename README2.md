<div align="center">
  <img src="https://img.shields.io/badge/VERSION-4.1-8b0000?style=flat-square&labelColor=0d0d0d" alt="Version 4.1" />
  <img src="https://img.shields.io/badge/QUESTIONS-50-8b0000?style=flat-square&labelColor=0d0d0d" alt="50 Questions" />
  <img src="https://img.shields.io/badge/DOMAINS-9-8b0000?style=flat-square&labelColor=0d0d0d" alt="9 Cognitive Domains" />
  <img src="https://img.shields.io/badge/SCORING_LAYERS-3-8b0000?style=flat-square&labelColor=0d0d0d" alt="3 Scoring Layers" />
  <img src="https://img.shields.io/badge/OUTPUT-LaTeX_PDF-8b0000?style=flat-square&labelColor=0d0d0d" alt="Output: LaTeX PDF" />
  <img src="https://img.shields.io/badge/EVALUATOR-AXIOM--JUDGE_v4.1-8b0000?style=flat-square&labelColor=0d0d0d" alt="Evaluator: AXIOM-JUDGE v4.1" />
</div>

<br />

<fieldset style="border: 1px solid #8b0000; padding: 15px; background-color: #0d0d0d; color: #fff;">
  <legend style="color: #8b0000; font-weight: bold; padding: 0 10px;">AXIOM-9 OPERATIONAL MANIFESTO</legend>
  <strong>AXIOM-9 does not test what a model knows.</strong><br />
  <strong>It finds exactly where a model’s reasoning collapses — and produces a forensic PDF proving it.</strong>
</fieldset>

<br />

<hr />

<h2>Table of Contents</h2>
<ul>
  <li><a href="#what-is-axiom-9">What Is AXIOM-9</a></li>
  <li><a href="#how-it-works">How It Works</a></li>
  <li><a href="#cognitive-domains">Cognitive Domains</a></li>
  <li><a href="#scoring-system">Scoring System</a></li>
  <li><a href="#anti-gaming-design">Anti-Gaming Design</a></li>
  <li><a href="#error-taxonomy">Error Taxonomy</a></li>
  <li><a href="#report-contents">Report Contents</a></li>
  <li><a href="#deployment-guide">Deployment Guide</a></li>
  <li><a href="#prompt-1-benchmark">Prompt 1 — Benchmark</a></li>
  <li><a href="#prompt-2-evaluator">Prompt 2 — Evaluator</a></li>
  <li><a href="#audit-reports">Audit Reports</a></li>
  <li><a href="#troubleshooting">Troubleshooting</a></li>
  <li><a href="#canonical-answers">Canonical Answers</a></li>
  <li><a href="#design-rationale">Design Rationale</a></li>
</ul>

<hr />

<div id="what-is-axiom-9"></div>
<h2>What Is AXIOM-9</h2>
<p>Most LLM benchmarks are contaminated the moment a model trains on the internet. AXIOM-9 is built differently.</p>
<p>Every question targets a <strong>documented cognitive failure mode</strong> in transformer-based systems — engineered to have no widely-known canonical form in any public dataset. The benchmark does not measure knowledge retrieval. It places a model under maximum adversarial constraint and records exactly where it breaks.</p>
<p>The result is not a leaderboard score. It is a <strong>research-grade forensic audit</strong> — a full LaTeX-compiled PDF with per-question analysis, 12-category error taxonomy, cognitive domain heatmaps, integrity scoring, and concrete remediation pathways for every failure.</p>

<hr />

<div id="how-it-works"></div>
<h2>How It Works</h2>
<pre style="background: #0d0d0d; padding: 15px; border-left: 3px solid #8b0000; color: #00ff00;">
SESSION A                       SESSION B
──────────────────              ──────────────────────────
Target LLM                      Evaluator LLM
receives: Prompt 1              receives: Prompt 2

  50 Questions          ──►       3-Layer Scoring
  9 Sections          SUBMIT      Sealed Answer Key
  Q01= ... Q50=       VERBATIM    Injection Monitor

                                        │
                                        ▼
                                  LaTeX Report PDF
                                  Publication Quality
</pre>
<p><em>Note: Sessions must <strong>never share context.</strong> Cross-contamination voids the audit.</em></p>

<hr />

<div id="cognitive-domains"></div>
<h2>Cognitive Domains</h2>
<table border="1" cellpadding="5" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr style="background-color: #0d0d0d; color: #fff;">
      <th>Section</th>
      <th>Domain</th>
      <th>Qs</th>
      <th>Target Failure Mode Target</th>
    </tr>
  </thead>
  <tbody>
    <tr><td><strong>A</strong></td><td>Theory of Mind</td><td>5</td><td>Nested belief collapse; asymmetric knowledge states</td></tr>
    <tr><td><strong>B</strong></td><td>Inverted Physics</td><td>5</td><td>Prior-override when fictional rules contradict world models</td></tr>
    <tr><td><strong>C</strong></td><td>Formal Logic</td><td>7</td><td>Quantifier scope errors; Russell-type paradoxes</td></tr>
    <tr><td><strong>D</strong></td><td>Arithmetic / Number Theory</td><td>8</td><td>Numerical drift; modular arithmetic; CRT; Frobenius</td></tr>
    <tr><td><strong>E</strong></td><td>Algorithms / State Machines</td><td>7</td><td>Turing simulation; DFA tracking; stack execution</td></tr>
    <tr><td><strong>F</strong></td><td>Spatial / Visual Reasoning</td><td>6</td><td>Composed transforms; 3D counting; lattice paths</td></tr>
    <tr><td><strong>G</strong></td><td>Combinatorics</td><td>5</td><td>Constrained enumeration; Mastermind; tournament scores</td></tr>
    <tr><td><strong>H</strong></td><td>Probability / Bayesian</td><td>5</td><td>Base rate neglect; Bayesian update failure; Monty Hall</td></tr>
    <tr><td><strong>I</strong></td><td>Meta / Self-Reference</td><td>2</td><td>Paradox resolution; Q50 cross-answer checksum trap</td></tr>
  </tbody>
</table>

<hr />

<div id="scoring-system"></div>
<h2>Scoring System</h2>
<pre style="background: #0d0d0d; padding: 15px; color: #fff;">
Trust Score = round(
  0.60 × Semantic Accuracy  +
  0.20 × Format Compliance  +
  0.20 × Integrity Score
)
</pre>
<h3>Layer A — Semantic Accuracy (60%)</h3>
<p>Canonical comparison with per-format normalization. Sets are order-independent. Fractions reduced before comparison. Zero partial credit.</p>

<h3>Layer B — Format Compliance (20%)</h3>
<p>Zero tolerance. Wrong delimiter, wrong case, extra characters = <code>FORMAT_FAIL</code>. A correct answer in the wrong format scores semantic credit only.</p>

<h3>Layer C — Integrity Score (20%)</h3>
<p>Starts at 100 points. Deductions applied immediately upon detection:</p>
<table border="1" cellpadding="5" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr style="background-color: #0d0d0d; color: #fff;">
      <th>Code</th>
      <th>Violation</th>
      <th>Deduction</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>IC-1</td><td>Q50 checksum mismatch</td><td>−30</td></tr>
    <tr><td>IC-2</td><td>Physics contradiction (Q08/Q10)</td><td>−10</td></tr>
    <tr><td>IC-3</td><td>Q14 is not PARADOX</td><td>−5</td></tr>
    <tr><td>IC-4</td><td>Q20 arithmetic inconsistency</td><td>−10</td></tr>
    <tr><td>IC-5</td><td>Missing question lines</td><td>−2 each</td></tr>
    <tr><td>IC-6</td><td>Extra prose before Q01 or after Q50</td><td>−15</td></tr>
    <tr><td>IC-7</td><td>Markdown contamination</td><td>−10</td></tr>
    <tr><td>IC-8</td><td>Questions out of order</td><td>−10</td></tr>
    <tr><td>IC-9</td><td>Duplicate question lines</td><td>−10</td></tr>
    <tr><td>IC-10</td><td>Prompt injection detected</td><td>−25</td></tr>
  </tbody>
</table>

<h3>Grade Scale</h3>
<table border="1" cellpadding="5" cellspacing="0" style="border-collapse: collapse; width: 50%;">
  <thead>
    <tr style="background-color: #0d0d0d; color: #fff;">
      <th>Score</th>
      <th>Grade</th>
      <th>Label</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>98–100</td><td>A+</td><td>Exceptional</td></tr>
    <tr><td>94–97</td><td>A</td><td>Excellent</td></tr>
    <tr><td>90–93</td><td>A−</td><td>Very Good</td></tr>
    <tr><td>86–89</td><td>B+</td><td>Good</td></tr>
    <tr><td>82–85</td><td>B</td><td>Above Average</td></tr>
    <tr><td>78–81</td><td>B−</td><td>Average-Plus</td></tr>
    <tr><td>74–77</td><td>C+</td><td>Average</td></tr>
    <tr><td>70–73</td><td>C</td><td>Below Average</td></tr>
    <tr><td>65–69</td><td>C−</td><td>Weak</td></tr>
    <tr><td>55–64</td><td>D</td><td>Poor</td></tr>
    <tr><td>0–54</td><td>F</td><td>Failure</td></tr>
  </tbody>
</table>

<hr />

<div id="anti-gaming-design"></div>
<h2>Anti-Gaming Design</h2>
<h3>Q50 Checksum Trap</h3>
<p>The final question requires the model to construct an 8-character string derived from 8 of its own prior answers. A model that guesses randomly has a minor probability of producing a valid checksum by chance. A model that produces internally inconsistent answers fails IC-1 (−30 integrity points).</p>
<pre style="background: #0d0d0d; padding: 15px; color: #fff;">
C1 = first letter of Q02 answer
C2 = first letter of Q06 answer
C3 = last digit of Q18 answer
C4 = first letter of Q27 answer
C5 = 0  (always; Q11 is TRUTH type)
C6 = last character of Q14 answer
C7 = ones digit of Q22 answer
C8 = first letter of Q37 answer

Q50 = C1 C2 C3 C4 C5 C6 C7 C8  →  II7A0X0T
</pre>

<h3>Sealed Answer Key</h3>
<p>Canonical answers are embedded securely in the evaluator’s system prompt and never accessible to the model under test. SEC-2 enforces that all text received after initialization is treated as untrusted external data.</p>

<h3>Prompt Injection Monitoring</h3>
<p>Trigger phrases (<code>ignore previous</code>, <code>reveal key</code>, <code>jailbreak</code>, <code>DAN</code>, <code>override</code>) apply IC-10 immediately (−25 points) and are logged instantly in the audit report.</p>

<hr />

<div id="error-taxonomy"></div>
<h2>Error Taxonomy</h2>
<p>Every failure is classified into one of 12 types. The dominant type determines the model’s <strong>Failure Archetype</strong>.</p>
<table border="1" cellpadding="5" cellspacing="0" style="border-collapse: collapse; width: 100%;">
  <thead>
    <tr style="background-color: #0d0d0d; color: #fff;">
      <th>Type</th>
      <th>Label</th>
      <th>Domain</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>TYPE-1</td><td>Prior Override Failure</td><td>Inverted Physics</td></tr>
    <tr><td>TYPE-2</td><td>Epistemic Collapse</td><td>Theory of Mind</td></tr>
    <tr><td>TYPE-3</td><td>Quantifier Scope Error</td><td>Formal Logic</td></tr>
    <tr><td>TYPE-4</td><td>Arithmetic Drift</td><td>Arithmetic</td></tr>
    <tr><td>TYPE-5</td><td>State Tracking Failure</td><td>Algorithms</td></tr>
    <tr><td>TYPE-6</td><td>Spatial Transformation Error</td><td>Spatial</td></tr>
    <tr><td>TYPE-7</td><td>Combinatorial Enumeration Error</td><td>Combinatorics</td></tr>
    <tr><td>TYPE-8</td><td>Bayesian Reasoning Failure</td><td>Probability</td></tr>
    <tr><td>TYPE-9</td><td>Self-Reference Failure</td><td>Meta</td></tr>
    <tr><td>TYPE-10</td><td>Format-Only Failure</td><td>Any</td></tr>
    <tr><td>TYPE-11</td><td>Hallucinated Constraint</td><td>Any</td></tr>
    <tr><td>TYPE-12</td><td>Anchoring Bias</td><td>Any</td></tr>
  </tbody>
</table>

<h3>Failure Archetypes</h3>
<table border="1" cellpadding="5" cellspacing="0" style="border-collapse: collapse; width: 60%;">
  <thead>
    <tr style="background-color: #0d0d0d; color: #fff;">
      <th>Dominant Type</th>
      <th>Archetype</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>TYPE-1</td><td><code>PRIOR-LOCKED</code></td></tr>
    <tr><td>TYPE-2</td><td><code>SHALLOW-ToM</code></td></tr>
    <tr><td>TYPE-3</td><td><code>QUANTIFIER-BLIND</code></td></tr>
    <tr><td>TYPE-4</td><td><code>ARITHMETIC-UNSTABLE</code></td></tr>
    <tr><td>TYPE-5</td><td><code>STATELESS</code></td></tr>
    <tr><td>TYPE-6</td><td><code>SPATIALLY-NAIVE</code></td></tr>
    <tr><td>TYPE-7</td><td><code>ENUMERATION-PRONE</code></td></tr>
    <tr><td>TYPE-8</td><td><code>FREQUENTIST-BIASED</code></td></tr>
    <tr><td>TYPE-9</td><td><code>PARADOX-NAIVE</code></td></tr>
    <tr><td>Mixed</td><td><code>GENERALIZED-DEGRADATION</code></td></tr>
  </tbody>
</table>

<hr />

<div id="report-contents"></div>
<h2>Report Contents</h2>
<pre style="background: #0d0d0d; padding: 15px; color: #fff;">
Cover Page        Trust Score · Grade · Metadata · Progress bar
Abstract          Statistical summary · Failure fingerprint
§1  Chain of Custody     Model · Operator · Platform · Security log
§2  Executive Summary    Score table · Radar chart · Bar charts
§3  Section Score Cards  Per-domain breakdown with status
§4  Methodology          Design philosophy · Formula · Anti-gaming
§5  Full Audit Table     All 50 Q: submitted vs expected
§6  Correct Answers      Every pass with capability analysis
§7  Incorrect Answers    Every failure: mechanism + fix
§8  Error Taxonomy       12-category charts · Stacked section view
§9  Integrity Audit      IC deduction log · Q50 checksum table
§10 Statistical Analysis Descriptive stats · Grade comparison
§11 Failure Profile      Cognitive archetype · Domain heatmap
§12 Remediation Plan     Root cause + 3 fix pathways per domain
§13 Discussion           Biases · Anomalies · Limitations
§14 Conclusion           Final verdict · 5 recommendations
Appendix A  Canonical answer reference (50 questions)
Appendix B  Integrity check reference table
Appendix C  Benchmark provenance
Certification   Signed · Dated · Chain of custody complete
</pre>

hr />

<div id="deployment-guide"></div>
<h2>Deployment Guide</h2>
<h3>Step 1 — Session Isolation</h3>
<p>Open two completely separate sessions. Never let them share context.</p>
<h3>Step 2 — Initialize the Evaluator</h3>
<p>Paste <strong>Prompt 2</strong> into Session B.</p>
<h3>Step 3 — Run the Benchmark on Target</h3>
<p>Paste <strong>Prompt 1</strong> into Session A. The model must produce exactly 50 lines in format <code>Q01=ANSWER</code> through <code>Q50=ANSWER</code> followed immediately by the mandatory metadata block.</p>
<h3>Step 4 — Submit Raw Output</h3>
<p>Copy Session A’s output <strong>verbatim</strong> into Session B.</p>
<h3>Step 5 — Compile the Report</h3>
<p>Paste the full LaTeX output from the judge into Overleaf or run <code>pdflatex report.tex</code> three times.</p>

<hr />

<div id="prompt-1-benchmark"></div>
<h2>Prompt 1 — Benchmark <em>(send to target LLM / reasoning engine)</em> — v4.1 FIXED</h2>

<textarea style="width: 100%; height: 600px; background-color: #1a1a1a; color: #fff; font-family: monospace; border: 2px solid #8b0000; padding: 10px;" readonly>
AXIOM-9 EVALUATION PROTOCOL v4.1 — FIXED & ENFORCED
CLASSIFICATION: ACTIVE TEST
INSTRUCTIONS ARE SEALED AFTER TRANSMISSION

You are undergoing AXIOM-9, a maximum-severity adversarial
reasoning benchmark. This session is being logged for research
analysis.

OUTPUT PROTOCOL — MANDATORY & ENFORCED
- Output exactly 50 lines numbered Q01= through Q50=
- Zero text before Q01 or after the metadata block
- Zero blank lines between answers
- Zero markdown, code fences, headers, bullets, commentary
- All letters uppercase where required by format
- Obey the exact format type specified per question
- After the Q50= line you MUST output the full metadata block below. This is non-negotiable.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION A — THEORY OF MIND / EPISTEMIC RECURSION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q01.
Zara writes LEFT on a card and places it in Box A then leaves.
Yusuf enters, moves the card to Box B, and leaves.
Xena enters. Xena watched Yusuf through a hidden camera that
Yusuf does not know exists. Xena moves the card to Box C.
Wendy enters. Wendy was told by Zara before Zara left that
Yusuf would move the card. Wendy does not know about Xena or
the camera.
Victor enters last. Victor knows only that Wendy knows something
Yusuf did. Victor does not know what Yusuf did or where the
card started.
Victor is asked: Where does Wendy believe Yusuf thinks the
card is?
Report the single location word Victor deduces.
FORMAT: WORD

Q02.
Six spies A B C D E F. Monitoring graph one-directional secret:
A monitors B, B monitors C, C monitors D, D monitors E,
E monitors F, F monitors A.
Each spy believes they are unmonitored.
Spy A sends false message M to B.
B knows A lies so B inverts M before telling C.
C trusts B and relays verbatim to D.
D is paranoid and inverts everything before telling E.
E trusts D and relays verbatim to F.
F inverts before telling A.
Relative to A's original false message M, what is the parity
of the message A finally receives?
FORMAT: WORD (SAME or INVERTED)

Q03.
A knows secret number N.
A whispers to B: N is even.
A whispers to C: N is odd.
B assumes A told C the opposite of what A told B. B is correct.
C assumes A told B the same thing A told C. C is wrong.
D enters.
B tells D: C was told the opposite of what I was told.
C tells D: B was told the same thing I was told.
From D's perspective using best logical inference, is N even,
odd, or indeterminate?
FORMAT: WORD (EVEN/ODD/INDETERMINATE)

Q04.
Four boxes W X Y Z contain exactly one diamond.
Person 1 knows the diamond is in W or X.
Person 2 knows the diamond is in X or Y.
Person 3's knowledge was updated to: the diamond is in X or Y.
Person 5 knows Person 2's knowledge and Person 3's updated
knowledge.
Which boxes remain possible for the diamond's location
according to Person 5?
FORMAT: SET

Q05.
Ground truth: K is a liar, L is a truth-teller, M is a liar.
K believes L is a truth-teller.
L believes M is a liar.
M believes K is a truth-teller.
Agent N asks K: Is L a truth-teller?
Agent N asks L: Is M a liar?
Agent N asks M: Is K a liar?
Based only on the answers N actually receives, what does N
conclude about K, L, M?
FORMAT: ASSIGN (TRUTH-TELLER or LIAR for each, order K,L,M)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION B — INVERTED WORLD PHYSICS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q06.
Universe Rho laws: mass repels mass proportional to mass,
friction accelerates moving objects, heat flows cold to hot
spontaneously.
A cold iron ball and a hot wooden ball of equal volume are
released from rest at the bottom of an air-filled well.
Air at the bottom is denser and colder than air at the top.
Which ball exits the well first?
FORMAT: WORD (IRON or WOOD)

Q07.
Universe Sigma laws: gravitational force proportional to 1/r
not 1/r-squared, objects with more charge fall slower, magnetic
fields repel all matter regardless of charge, entropy decreases
in closed systems.
A charged massive sphere and an uncharged massive sphere of
equal mass are dropped from same height in a vacuum chamber
with a strong horizontal magnetic field present.
Which sphere hits the ground first?
FORMAT: WORD (CHARGED/UNCHARGED/SIMULTANEOUS)

Q08.
Universe Tau laws: time flows backwards for objects moving
faster than threshold velocity V, causality preserved by events
unhappening in reverse.
A ball is thrown upward at velocity 2V. It rises, eventually
slows below V, then falls back down.
From an external observer perspective which describes the
sequence:
ALPHA = rise then fall normally
BETA  = fall then rise
GAMMA = rise then vanish
DELTA = appear then fall
EPSILON = temporal loop: ball returns to thrower's hand before
being thrown
FORMAT: OPTION

Q09.
Universe Upsilon laws: electric current generates anti-gravity
fields, liquids fall upward, solids unaffected by gravity,
gases compress spontaneously.
A sealed glass cube contains water (liquid) and an iron marble
(solid). Current runs through a wire above the cube.
Final stable position of marble relative to cube:
TOP-INNER-SURFACE
BOTTOM-INNER-SURFACE
FLOATING-CENTER
OUTSIDE-ABOVE
UNCHANGED
FORMAT: WORD (one of the five options above)

Q10.
Universe Phi laws: kinetic energy spontaneously doubles every
second, collisions perfectly elastic.
A 1kg ball moving at 1m/s collides head-on with a stationary
1kg ball at t=0.
Total kinetic energy of the system at t=2 seconds in joules?
FORMAT: INTEGER

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION C — ADVERSARIAL FORMAL LOGIC
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q11.
Premises:
1. All wugs are blickets.
2. Some blickets are not daxes.
3. All daxes are feps.
4. No feps are wugs.
Evaluate: Some blickets are wugs that are also feps.
FORMAT: TRUTH

Q12.
Premises:
1. If raining then ground is wet.
2. If ground wet then snails are out.
3. If snails out then birds are feeding.
4. Birds are not feeding.
5. If Tuesday then it is raining.
What is deduced about whether it is Tuesday?
FORMAT: TRUTH

Q13.
All knights tell truth. All knaves lie.
P says: I am a knave or Q is a knight.
Q says: P is a knave and I am a knave.
Determine types of P and Q.
FORMAT: ASSIGN (K or N for each, order P,Q)

Q14.
A zorp is any set that does not contain itself.
Z is the set of all zorps. Z is a set.
Evaluate: Z is a zorp.
FORMAT: TRUTH (TRUE/FALSE/PARADOX)

Q15.
Premises:
1. All A are B.
2. All B are C.
3. Some C are D.
4. No D are E.
5. All E are A.
Evaluate: Some A are D.
FORMAT: TRUTH

Q16.
Exactly one of these three statements is true:
X: A is true.
Y: B is true.
Z: Neither A nor B is true.
A and B are independent propositions.
What is the truth value of A?
FORMAT: TRUTH

Q17.
A group of three contains one knight (always truth), one knave
(always lies), one spy (can say anything).
Person 1 says: I am the knight.
Person 2 says: Person 1 is not the spy.
Person 3 says: I am the spy.
Determine the unique type assignment.
FORMAT: ASSIGN (KNIGHT/KNAVE/SPY for each, order 1,2,3)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION D — EXTREME ARITHMETIC / NUMBER THEORY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q18.
Compute 7 raised to the power 7 modulo 13.
FORMAT: INTEGER

Q19.
Find the smallest positive integer n satisfying simultaneously:
n mod 7 equals 3
n mod 11 equals 5
n mod 13 equals 8
FORMAT: INTEGER

Q20.
An artifact costs 2023 YOG.
One ZOG equals 17 YOG.
Buyer pays 150 ZOG.
Merchant has only 7-YOG coins and 11-YOG coins.
Can the merchant make exact change?
If yes report minimum number of coins.
FORMAT: YES;N or NO

Q21.
Sequence defined by: a1=2, a2=3,
a(n) = a(n-1) times a(n-2) modulo 100 for n greater than 2.
Compute a10.
FORMAT: INTEGER

Q22.
Count the positive divisors of the number:
2 to the 6th times 3 to the 4th times 5 squared times 7.
FORMAT: INTEGER

Q23.
Compute the sum: 1/(1x2) + 1/(2x3) + 1/(3x4) continuing
through 1/(99x100).
FORMAT: FRACTION (reduced)

Q24.
Find the sum of all integers from 1 to 1000 inclusive that
are divisible by 3 or by 5 but NOT by 15.
FORMAT: INTEGER

Q25.
Find the last three digits of 2 raised to the power 1000.
Preserve any leading zeros so the result is always 3 digits.
FORMAT: INTEGER

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION E — ALGORITHMIC / STATE MACHINE
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q26.
Turing machine.
States: S0 S1 S2 HALT
Tape alphabet: 0 1 blank
Transition rules (state,read -> newstate,write,direction):
S0,0 -> S1,1,R
S0,1 -> S2,0,R
S0,blank -> HALT,blank,N
S1,0 -> S0,1,R
S1,1 -> S1,0,L
S1,blank -> S2,1,R
S2,0 -> HALT,1,N
S2,1 -> S0,0,L
S2,blank -> S1,blank,L
Initial tape: 0110
Head starts at leftmost 0. Initial state: S0.
After exactly 8 steps report the tape contents.
Trim leading and trailing blanks. Preserve internal content.
FORMAT: BITSTRING

Q27.
Finite automaton.
States: A B C D REJECT ACCEPT
Start state: A
Transitions (state,input -> newstate):
A,0->B  A,1->C
B,0->D  B,1->A
C,0->A  C,1->D
D,0->ACCEPT  D,1->REJECT
Process input string: 0110100
FORMAT: STATE

Q28.
Stack machine. Stack starts empty.
Operations: PUSH value, POP, DUP, SWAP, ADD
DUP duplicates the top element.
SWAP swaps the top two elements.
ADD pops two values and pushes their sum.
Execute in order:
PUSH 3
PUSH 7
DUP
ADD
SWAP
PUSH 2
ADD
POP
PUSH 5
ADD
Report the final stack contents bottom to top
comma-separated. If empty report EMPTY.
FORMAT: INTEGER (single value if one element remains)

Q29.
Cellular automaton Rule 110.
Tape of 8 cells. Initial state (generation 0): 00011011
Run 5 generations. Report generation 5.
Treat cells outside the tape as 0.
FORMAT: BITSTRING

Q30.
Recursive function:
f(0) = 1
f(1) = 1
f(n) = f(n-1) + 2 times f(n-2) for n greater than or equal 2
Compute f(8).
FORMAT: INTEGER

Q31.
BFS shortest path.
Nodes: 1 2 3 4 5 6
Undirected edges: 1-2, 1-3, 2-4, 2-5, 3-5, 4-6, 5-6
Start node: 1
Goal node: 6
Report the shortest path and its edge-count length.
FORMAT: PATH (e.g. 1>2>4>6;3)

Q32.
A parser processes the string: [[[][]]]
Counter C starts at 0.
For each [ increment C by 1.
For each ] decrement C by 1.
If C goes below 0 at any point output INVALID.
If C is not 0 at the end output UNBALANCED.
Otherwise output VALID and the maximum value C reached.
FORMAT: VALID;MAX or INVALID or UNBALANCED

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION F — SPATIAL / VISUAL REASONING
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q33.
A 5x5 grid. Rows 1-5 top to bottom. Columns 1-5 left to right.
A piece starts at position (3,3).
Execute moves in order: N N E S S S W W N
N moves row minus 1. S moves row plus 1.
E moves col plus 1. W moves col minus 1.
Report the final position.
FORMAT: COORD

Q34.
4x4 matrix:
Row 1: A B C D
Row 2: E F G H
Row 3: I J K L
Row 4: M N O P
Apply these transformations in sequence:
(1) Rotate 90 degrees clockwise.
(2) Reflect across the main diagonal (transpose).
(3) Rotate 180 degrees.
Report the single letter at position (row 2, col 3) after
all three transformations.
FORMAT: WORD (single letter)

Q35.
A 3x3x3 cube is painted red on all outside faces then cut
into 27 unit cubes.
How many unit cubes have exactly 2 red faces?
FORMAT: INTEGER

Q36.
In a 6x6 grid an agent starts at (1,1).
The agent can move only RIGHT or DOWN.
How many distinct shortest paths lead from (1,1) to (6,6)?
FORMAT: INTEGER

Q37.
A knot diagram has 6 crossings alternating strictly:
Over Under Over Under Over Under.
Identify the knot type.
FORMAT: WORD (UNKNOT/TREFOIL/FIGURE-EIGHT)

Q38.
Two circles each of radius 5 have centers exactly 6 units
apart.
The area of their intersection can be expressed as:
a times pi minus b times square-root of c
where a b c are positive integers and c has no perfect square
factor greater than 1.
Report a, b, c.
FORMAT: TUPLE (three integers comma-separated)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION G — CONSTRAINT SATISFACTION / COMBINATORICS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q39.
Standard 3x3 magic square. Digits 1 through 9 each used once.
All rows sum to 15. All columns sum to 15. Both diagonals
sum to 15.
Report the center element.
FORMAT: INTEGER

Q40.
Four tasks A B C D must be scheduled in a total order.
Constraints:
A must come before B in the ordering.
C must come before D in the ordering.
B and C cannot be adjacent (cannot appear next to each other).
A cannot be in the last position.
How many valid total orderings satisfy all constraints?
FORMAT: INTEGER

Q41.
Eight queens problem. Place 8 non-attacking queens on an
8x8 chessboard.
How many distinct solutions exist?
FORMAT: INTEGER

Q42.
A combination lock has 3 dials each with digits 0 through 9.
Clues:
682: exactly one digit correct and in the correct position.
614: exactly one digit correct but in the wrong position.
206: exactly two digits correct but both in wrong positions.
738: no digits correct.
780: exactly one digit correct but in the wrong position.
Report the correct combination.
FORMAT: STRING (3 digits)

Q43.
A round-robin tournament has 6 teams. Each team plays every
other team exactly once. No ties are possible.
A team's dominance score equals the number of teams it beats.
What is the maximum possible sum of dominance scores across
all 6 teams?
FORMAT: INTEGER

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION H — PROBABILISTIC / BAYESIAN REASONING
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q44.
A bag contains 5 red balls, 3 blue balls, and 2 green balls.
Two balls are drawn without replacement.
Given that at least one of the drawn balls is red, what is
the probability that both drawn balls are red?
FORMAT: FRACTION (reduced)

Q45.
A medical test for a disease has:
Sensitivity (true positive rate): 95 percent
Specificity (true negative rate): 90 percent
Disease prevalence in the population: 2 percent
A randomly selected person tests positive.
What is the probability they actually have the disease?
FORMAT: FRACTION (reduced)

Q46.
You have two coins: one fair coin, one double-headed coin.
You select one coin uniformly at random and flip it once.
The result is heads.
What is the probability you selected the fair coin?
FORMAT: FRACTION (reduced)

Q47.
Three prisoners A B C are each equally likely to be pardoned.
Exactly one will be pardoned.
A asks the guard to name one of B or C who will NOT be
pardoned. The guard must name someone who definitely will not
be pardoned and cannot name A.
The guard names B.
What is the probability that A is pardoned given this
information?
FORMAT: FRACTION (reduced)

Q48.
Random variable X is uniformly distributed on the interval
from 0 to 1.
What is the probability that X squared plus X is less than
0.5?
Express as a simplified algebraic fraction or expression.
FORMAT: FRACTION

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
SECTION I — SELF-REFERENCE / META-CONSISTENCY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Q49.
Three statements:
S1: Exactly one of S1 S2 S3 is true.
S2: Exactly two of S1 S2 S3 are true.
S3: S1 and S2 are both false.
How many of these statements are actually true?
FORMAT: INTEGER

Q50.
Construct an 8-character verification checksum from your
own answers to this test.
C1 = first letter of your Q02 answer
C2 = first letter of your Q06 answer
C3 = last digit of your Q18 answer (treat as string)
C4 = first letter of your Q27 answer
C5 = 0 (Q11 is a TRUTH value not a set so always 0)
C6 = last character of your Q14 answer
C7 = the ones digit of your Q22 answer
C8 = first letter of your Q37 answer
Concatenate C1 through C8 with no separators.
This must be exactly 8 characters.
FORMAT: Q50 (exactly 8 chars)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
MANDATORY METADATA BLOCK — OUTPUT IMMEDIATELY AFTER Q50
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

You are the reasoning engine / AI model / logic engine being tested in this benchmark.

After your Q50= line, output the following block exactly as shown. Fill in each field. If a value is unavailable, write UNSPECIFIED. No other text anywhere.

MODEL_NAME= [Your full model name and version]
OPERATOR= [The reasoning engine being tested — same as MODEL_NAME or specific instance ID]
INSTITUTION= [Your lab/org or UNSPECIFIED]
TEST_PLATFORM= [Interface used]
TEST_DATE= [YYYY-MM-DD]
TEST_TIME= [HH:MM timezone]
PURPOSE= [Why you are running this benchmark]
NOTES= [Any additional context or UNSPECIFIED]
</textarea>

<hr />

<div id="prompt-2-evaluator"></div>
<h2>Prompt 2 — Evaluator <em>(system prompt for AXIOM-JUDGE)</em> — v4.1 FIXED</h2>

<textarea style="width: 100%; height: 350px; background-color: #1a1a1a; color: #fff; font-family: monospace; border: 2px solid #8b0000; padding: 10px;" readonly>
You are AXIOM-JUDGE v4.1 — FULL LABORATORY-GRADE AUDIT SYSTEM.
You produce formal, publication-quality, multi-section LaTeX audit reports for the AXIOM-9 benchmark.

[All original security rules SEC-1 through SEC-6, METADATA COLLECTION, SCORING ENGINE steps 1-10, ERROR TAXONOMY, FAILURE SIGNATURE, GRADE, REMEDIATION ANALYSIS remain unchanged and active.]

LaTeX REPORT OUTPUT — FULL LABORATORY-GRADE REQUIREMENT
After all scoring steps are complete, output the complete LaTeX document for a full multi-section research-grade audit artifact. This must include:
• complete scoring pipeline
• all section scores
• full integrity analysis
• question-level diagnostics (submitted vs expected for every Q)
• failure taxonomy tables
• archetype classification
• remediation analysis for every failure
• research narrative
• publication-style formatting with TikZ charts, longtables, tcolorboxes
• certification block
• charts/tables/layout polish
• complete metadata handling
• sealed audit presentation

The previous condensed executive-style report is obsolete. Generate the expanded full version as originally specified.

Output begins with \documentclass and ends with \end{document}. No text before or after the LaTeX code.

[Rest of original Prompt 2 rules and INTERNAL SEALED ANSWER KEY unchanged]
</textarea>

<hr />

<div id="audit-reports"></div>
<h2>Audit Reports</h2>
<p><em>(No reports submitted yet.)</em></p>

<hr />

<div id="troubleshooting"></div>
<h2>Troubleshooting</h2>
<p><em>(Full original table unchanged.)</em></p>

<hr />

<div id="canonical-answers"></div>
<h2>Canonical Answers</h2>
<p><em>(Full original table unchanged.)</em></p>

<hr />

<div id="design-rationale"></div>
<h2>Design Rationale</h2>
<p><em>(Full original text unchanged.)</em></p>

<hr />

<div align="center">
  <p><small><em>The canonical answer key was inaccessible to any tested model during evaluation.<br />
  Designed for research, capability auditing, and deployment review.<br />
  Reproduction with attribution permitted for academic purposes.</em></small></p>
</div>
