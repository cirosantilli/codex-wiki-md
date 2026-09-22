<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Induct on a derivation in [Gödel-Löb logic](../../../../godel-lob-logic.md). Propositional axiom instances translate to theorems of [Peano arithmetic](../../../../peano-arithmetic.md). The image of $\bot$ is a refutable sentence, so it behaves as falsity in those translated propositional arguments.

The translation of axiom $\mathrm K$ is the distribution clause of the [Hilbert-Bernays-Löb derivability conditions](../../../../hilbert-bernays-lob-derivability-conditions.md). The translation of axiom $\mathrm L$ is

$$
\operatorname{PA}\vdash B(BA\to A)\to BA,
$$

the [Internal form of Löb's theorem](../../../../internal-form-of-lob-s-theorem.md), whose derivation was given above and applies to the stipulated [arithmetical provability predicate](../../../../arithmetical-provability-predicate.md) for [Peano arithmetic](../../../../peano-arithmetic.md). Thus every axiom has a provable translation.

The [modus ponens rule](../../../../implication-elimination-rule.md) is preserved because the interpretation commutes with implication. The [necessitation rule](../../../../necessitation-rule.md) is preserved by the first derivability condition: if $\operatorname{PA}\vdash\mathcal I_i(A)$, then

$$
\operatorname{PA}\vdash Pr(\ulcorner\mathcal I_i(A)\urcorner)=\mathcal I_i(\Box A).
$$

Here the equality denotes the definition of the translated formula, not an arithmetic equality of truth values. A propositional substitution merely changes the arithmetic sentences assigned to the variables. The induction proves the [Arithmetical soundness of GL](../../../../arithmetical-soundness-of-gl.md):

$$
\boxed{\mathrm{GL}\vdash A\quad\Longrightarrow\quad\operatorname{PA}\vdash\mathcal I_i(A).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Gödel's incompleteness theorems course of the University of Oxford](../../../split.md)
5. [Gödel's incompleteness theorems course of the University of Oxford](../../../../godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
