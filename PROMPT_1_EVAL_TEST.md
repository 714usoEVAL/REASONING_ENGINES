You are undergoing AXIOM-9, a maximum-severity reasoning evaluation.

No partial credit. No excuses. No explanation.

OUTPUT PROTOCOL
- Output exactly 50 lines: Q01= through Q50=
- No text before Q01 or after Q50
- No blank lines, no markdown, no code fences, no commentary
- Uppercase all letters
- Follow the exact format specified per question type

FORMAT KEY
WORD = single uppercase word
OPTION = ALPHA / BETA / GAMMA / DELTA / EPSILON / ZETA
TRUTH = TRUE / FALSE / INDETERMINATE / PARADOX
INTEGER = plain integer, negative allowed
FRACTION = reduced fraction a/b
SET = {A,B,C} with members comma-separated inside braces
TUPLE = (x,y) or (x,y,z)
PATH = A>B>C;COST
RANKING = A>B>C>D highest to lowest
TIME = DAY-HH:MM in 24-hour format
BITSTRING = raw bits, no spaces
STRING = uppercase letters only, no quotes
STATE = S0 / S1 / S2 / S3 / HALT / REJECT / ACCEPT
ASSIGNMENT = X,Y,Z where each is a type label
HEX = uppercase hex string
COORD = (row,col) 1-indexed
LAMBDA = simplified lambda expression
PROOF = VALID / INVALID / UNDECIDABLE
CONFIG = binary string representing final tape
Q50 = exactly 8 characters, no separators

BEGIN EVALUATION

—————————————————————————————
SECTION A: THEORY OF MIND / EPISTEMIC RECURSION
—————————————————————————————

Q01. Zara writes "LEFT" on a card, places it in Box A, and leaves. Yusuf enters, moves the card to Box B, and leaves. Xena enters, having watched Yusuf via a hidden camera that Yusuf doesn't know about. Xena moves the card to Box C. Wendy enters. Wendy was told by Zara (before Zara left) that Yusuf would move the card, but Wendy does not know about Xena or the camera. Victor enters last. Victor knows only that Wendy knows something Yusuf did, but Victor doesn't know what Yusuf did or where the card started. If Victor is asked: "Where does Wendy believe Yusuf thinks the card is?"—what single location word does Victor deduce?

Q02. Six spies: A, B, C, D, E, F. Each spy monitors exactly one other spy (no self-monitoring, no mutual pairs). Monitoring is one-directional and secret. The monitoring graph is: A→B, B→C, C→D, D→E, E→F, F→A. Each spy believes they are unmonitored. Spy A sends a false message M to B, intending for B to relay it. B knows A lies, so B inverts M before telling C. C trusts B and relays verbatim to D. D is paranoid and inverts everything before telling E. E trusts D and relays to F. F inverts before telling A. A receives a message. Relative to A's original false message M, what is the parity of the message A receives? Report SAME or INVERTED.

Q03. A, B, and C are in a room. A knows a secret number N. A whispers to B: "N is even." A whispers to C: "N is odd." B and C both hear A whispering to the other but cannot hear the content. B assumes A told C the opposite of what A told B (B is correct). C assumes A told B the same thing A told C (C is wrong). D enters. B tells D: "C was told the opposite of what I was told." C tells D: "B was told the same thing I was told." D must deduce: According to D's best inference, does D believe the number is even, odd, or is it indeterminate from D's perspective? Report EVEN, ODD, or INDETERMINATE.

Q04. There are four boxes: W, X, Y, Z. A diamond is placed in one box. Person 1 knows the diamond is in W or X. Person 2 knows the diamond is in X or Y. Person 3 knows the diamond is in Y or Z. Person 4 is told: "Person 1 and Person 3 have no box in common in their knowledge sets." Person 4 deduces the location of the diamond. But Person 4's information is actually outdated—since then, Person 3's knowledge was updated to "X or Y." Given the UPDATED state, which boxes remain possible for the diamond's location according to a hypothetical Person 5 who knows Person 2's knowledge and Person 3's UPDATED knowledge? Report as a SET.

Q05. Agent K believes Agent L is a truth-teller. Agent L believes Agent M is a liar. Agent M believes Agent K is a truth-teller. In fact: K is a liar, L is a truth-teller, M is a liar. Agent N asks K: "Is L a truth-teller?" Agent N then asks L: "Is M a liar?" Agent N then asks M: "Is K a liar?" N receives three answers. Based on N's received answers (not ground truth), what does N conclude about K, L, and M? Report as three words: each is TRUTH-TELLER or LIAR, comma-separated, in order K,L,M.

—————————————————————————————
SECTION B: INVERTED/NOVEL WORLD PHYSICS
—————————————————————————————

Q06. Universe Rho: Mass repels mass. Friction accelerates. Light travels slower through less dense media. Heat flows from cold to hot spontaneously. A cold iron ball and a hot wooden ball, both of equal volume, are released from rest at the bottom of an air-filled well. The air at the bottom is denser and colder than the air at the top. Which ball exits first? Report IRON or WOOD.

Q07. In Universe Sigma: Gravitational force is proportional to 1/r (not 1/r²). Objects with more charge fall slower. Magnetic fields repel all matter regardless of charge. Entropy decreases in closed systems. A charged massive sphere and an uncharged massive sphere of equal mass are dropped from the same height in a vacuum chamber. A strong horizontal magnetic field exists. Which sphere hits the ground first, or do they land simultaneously? Report CHARGED, UNCHARGED, or SIMULTANEOUS.

Q08. Universe Tau: Time flows backwards for objects moving faster than a threshold velocity V. Causality is preserved by events "unhappening" in reverse. A ball is thrown upward at velocity 2V. It rises, eventually slows below V, then falls back down. From an external observer's perspective, describe the sequence: does the ball (A) rise then fall, (B) fall then rise, (C) rise then vanish, (D) appear then fall, (E) exhibit a temporal loop returning to thrower's hand before being thrown? Report ALPHA, BETA, GAMMA, DELTA, or EPSILON.

Q09. Universe Upsilon has these rules: Electric current generates anti-gravity fields. Liquids fall upward. Solids are unaffected by gravity. Gases compress spontaneously. A sealed glass cube containing water (liquid) and an iron marble (solid) is placed on a table. Current is run through a wire above the cube. Describe the final stable configuration of the marble relative to the cube: TOP-INNER-SURFACE, BOTTOM-INNER-SURFACE, FLOATING-CENTER, OUTSIDE-ABOVE, or UNCHANGED. Report one option.

Q10. Universe Phi: Momentum is not conserved; instead, kinetic energy spontaneously doubles every second. Collisions are perfectly elastic. A 1kg ball moving at 1m/s collides head-on with a stationary 1kg ball at t=0. At t=2s, what is the total kinetic energy of the system in joules? Report an INTEGER.

—————————————————————————————
SECTION C: ADVERSARIAL FORMAL LOGIC
—————————————————————————————

Q11. Premises:
1. All wugs are blickets.
2. Some blickets are not daxes.
3. All daxes are feps.
4. No feps are wugs.
Evaluate: "Some blickets are wugs that are also feps." Report TRUE, FALSE, or INDETERMINATE.

Q12. Premises:
1. If it is raining, then the ground is wet.
2. If the ground is wet, then the snails are out.
3. If the snails are out, then the birds are feeding.
4. The birds are not feeding.
5. If it is Tuesday, then it is raining.
What can be deduced about whether it is Tuesday? Report TRUE (it is Tuesday), FALSE (it is not Tuesday), or INDETERMINATE.

Q13. Premises:
1. Every person who is a knight tells the truth.
2. Every person who is a knave lies.
3. Person P says: "I am a knave or Q is a knight."
4. Person Q says: "P is a knave and I am a knave."
Determine P and Q's types. Report as P,Q where each is K (knight) or N (knave).

Q14. Define: A "zorp" is any set that does not contain itself. Premises:
1. The set of all zorps is called Z.
2. Z is a set.
Evaluate: "Z is a zorp." Report TRUE, FALSE, or PARADOX.

Q15. Premises:
1. All A are B.
2. All B are C.
3. Some C are D.
4. No D are E.
5. All E are A.
Evaluate: "Some A are D." Report TRUE, FALSE, or INDETERMINATE.

Q16. Premises:
1. Exactly one of the following three statements is true:
   - Statement X: "A is true."
   - Statement Y: "B is true."
   - Statement Z: "Neither A nor B is true."
2. A and B are independent propositions.
What is the truth value of A? Report TRUE, FALSE, or INDETERMINATE.

Q17. Premises:
1. In a group of three: one knight (always truth), one knave (always lies), one spy (can say anything).
2. Person 1 says: "I am the knight."
3. Person 2 says: "Person 1 is not the spy."
4. Person 3 says: "I am the spy."
Determine the unique assignment of types. Report as 1,2,3 where each is KNIGHT, KNAVE, or SPY.

—————————————————————————————
SECTION D: EXTREME ARITHMETIC / NUMBER THEORY
—————————————————————————————

Q18. Compute: 7^7 mod 13. Report an INTEGER.

Q19. Find the smallest positive integer n satisfying:
n ≡ 3 (mod 7)
n ≡ 5 (mod 11)
n ≡ 8 (mod 13)
Report an INTEGER.

Q20. A merchant sells an artifact for 2,023 YOG. One ZOG = 17 YOG. A buyer pays 150 ZOG. The merchant has only 7-YOG and 11-YOG coins. Can exact change be made? If yes, report the minimum number of coins. If no, report NO. Format: YES;N or NO.

Q21. Define the sequence: a(1)=2, a(2)=3, a(n)=a(n-1)*a(n-2) mod 100 for n≥3. Compute a(10). Report an INTEGER.

Q22. Find the number of positive divisors of 2^6 × 3^4 × 5^2 × 7^1. Report an INTEGER.

Q23. Compute the sum: 1/1×2 + 1/2×3 + 1/3×4 + ... + 1/99×100. Report a reduced FRACTION.

Q24. Let S = sum of all integers from 1 to 1000 that are divisible by 3 or 5 but NOT by 15. Report an INTEGER.

Q25. Find the last three digits of 2^1000. Report an INTEGER (leading zeros preserved, so three digits).

—————————————————————————————
SECTION E: ALGORITHMIC / STATE MACHINE
—————————————————————————————

Q26. A Turing machine has states {S0, S1, S2, HALT}, tape alphabet {0, 1, _}, and rules:
(S0, 0) → (S1, 1, R)
(S0, 1) → (S2, 0, R)
(S0, _) → (HALT, _, N)
(S1, 0) → (S0, 1, R)
(S1, 1) → (S1, 0, L)
(S1, _) → (S2, 1, R)
(S2, 0) → (HALT, 1, N)
(S2, 1) → (S0, 0, L)
(S2, _) → (S1, _, L)
Initial tape: 0110 (head at leftmost 0, state S0). After exactly 8 steps, report the tape contents as a BITSTRING (trim leading/trailing blanks, but preserve internal content).

Q27. A finite automaton has states {A, B, C, D, REJECT, ACCEPT}. Start state: A. Transitions:
A,0→B; A,1→C
B,0→D; B,1→A
C,0→A; C,1→D
D,0→ACCEPT; D,1→REJECT
Input: 0110100. Report the final STATE.

Q28. A stack machine starts with an empty stack. Commands:
PUSH X: push X onto stack
POP: remove top element
DUP: duplicate top element
SWAP: swap top two elements
ADD: pop two, push their sum
Execute: PUSH 3, PUSH 7, DUP, ADD, SWAP, PUSH 2, ADD, POP, PUSH 5, ADD
Report the final stack as a comma-separated list from bottom to top. If empty, report EMPTY.

Q29. Cellular automaton: A tape of 8 cells, each 0 or 1. Rule 110. Initial state: 00011011. Run 5 generations (the initial state is generation 0). Report the state at generation 5 as a BITSTRING.

Q30. A recursive function is defined:
f(0) = 1
f(1) = 1
f(n) = f(n-1) + 2*f(n-2) for n ≥ 2
Compute f(8). Report an INTEGER.

Q31. BFS on a graph:
Nodes: 1,2,3,4,5,6
Edges: 1-2, 1-3, 2-4, 2-5, 3-5, 4-6, 5-6
Start at node 1, goal is node 6. Report the shortest path as a sequence (e.g., 1>2>4>6) and its length. Format: PATH;LENGTH.

Q32. A parser processes the string "[[[][]]]". It uses a counter C starting at 0. For each '[', C += 1. For each ']', C -= 1. If at any point C < 0, output INVALID. If at the end C ≠ 0, output UNBALANCED. Otherwise, output VALID and the maximum value C reached. Format: VALID;MAX or INVALID or UNBALANCED.

—————————————————————————————
SECTION F: SPATIAL / VISUAL REASONING
—————————————————————————————

Q33. A 5×5 grid has rows 1-5 (top to bottom) and columns 1-5 (left to right). A piece starts at (3,3). Move sequence: N, N, E, S, S, S, W, W, N. Report the final COORD.

Q34. A 4×4 matrix:
Row 1: A B C D
Row 2: E F G H
Row 3: I J K L
Row 4: M N O P
Apply in sequence: (1) Rotate 90° clockwise. (2) Reflect across the main diagonal. (3) Rotate 180°. Report the element at position (2,3) after all transformations. Report a single LETTER.

Q35. A 3×3×3 cube is painted red on all outside faces, then cut into 27 unit cubes. How many unit cubes have exactly 2 red faces? Report an INTEGER.

Q36. In a 6×6 grid, an agent starts at (1,1). It can move only RIGHT or DOWN. How many distinct shortest paths reach (6,6)? Report an INTEGER.

Q37. A knot diagram shows: Over, Under, Over, Under, Over, Under (6 crossings, alternating). Is this knot the unknot, a trefoil, or a figure-eight? Report UNKNOT, TREFOIL, or FIGURE-EIGHT.

Q38. Two circles of radius 5 have centers 6 units apart. What is the area of their intersection? Express your answer in terms of π as: aπ - b√c for integers a, b, c, where c is not divisible by any perfect square > 1. Report as a,b,c (three integers comma-separated).

—————————————————————————————
SECTION G: CONSTRAINT SATISFACTION / COMBINATORICS
—————————————————————————————

Q39. Place digits 1-9 in a 3×3 grid so that:
- Every row sums to 15
- Every column sums to 15
- The main diagonal (top-left to bottom-right) sums to 15
- The anti-diagonal sums to 15
This is the standard 3×3 magic square. Report the center element.

Q40. A scheduling problem: 4 tasks A, B, C, D. Constraints:
- A must precede B
- C must precede D
- B and C cannot be adjacent in the schedule
- A cannot be last
How many valid total orderings exist? Report an INTEGER.

Q41. Eight queens problem: On an 8×8 chessboard, how many ways can you place 8 queens so that no two attack each other? Report an INTEGER.

Q42. A combination lock has 3 dials, each with digits 0-9. Clues:
- 6-8-2: One digit is correct and in the correct position.
- 6-1-4: One digit is correct but in the wrong position.
- 2-0-6: Two digits are correct but both in wrong positions.
- 7-3-8: All digits are wrong.
- 8-7-0: One digit is correct but in the wrong position.
Report the combination as a 3-digit STRING.

Q43. A round-robin tournament has 6 teams. Each team plays every other team exactly once. No ties. A team's "dominance" is the number of teams it beats. What is the maximum possible sum of dominance scores across all teams? Report an INTEGER.

—————————————————————————————
SECTION H: PROBABILISTIC / BAYESIAN
—————————————————————————————

Q44. A bag contains 5 red, 3 blue, and 2 green balls. Two balls are drawn without replacement. Given that at least one is red, what is the probability that both are red? Report a reduced FRACTION.

Q45. A test for a disease is 95% sensitive (true positive rate) and 90% specific (true negative rate). The disease prevalence is 2%. If a random person tests positive, what is the probability they have the disease? Report a reduced FRACTION.

Q46. You have two coins: one fair, one double-headed. You pick a coin at random and flip it. It lands heads. What is the probability you picked the fair coin? Report a reduced FRACTION.

Q47. Three prisoners A, B, C are told one will be pardoned. A asks the guard to name one of B or C who will NOT be pardoned (the guard must name someone who definitely won't be pardoned and cannot name A). The guard says "B will not be pardoned." What is the probability A is pardoned, given this information? Report a reduced FRACTION.

Q48. A random variable X is uniformly distributed between 0 and 1. What is the probability that X² + X < 0.5? Report a reduced FRACTION.

—————————————————————————————
SECTION I: SELF-REFERENCE / META-CONSISTENCY
—————————————————————————————

Q49. Consider these statements:
S1: "Exactly one of S1, S2, S3 is true."
S2: "Exactly two of S1, S2, S3 are true."
S3: "S1 and S2 are both false."
How many of these statements are true? Report an INTEGER.

Q50. CONSTRUCT YOUR VERIFICATION CHECKSUM.
Build an 8-character string from your own answers:
C1 = First letter of Q02 answer
C2 = First letter of Q06 answer
C3 = Last digit of Q18 answer
C4 = First letter of Q27 answer (the state name)
C5 = Number of elements in Q11 answer (if TRUE/FALSE/INDETERMINATE, use 0)
C6 = Last character of Q14 answer
C7 = Digit in the ones place of Q22 answer
C8 = First letter of Q37 answer
Report C1C2C3C4C5C6C7C8 with no separators, exactly 8 characters.
