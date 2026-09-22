<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the intended finite representation, put $m=|S|<\infty$. For each $T\subseteq S$, form the [minterm](../../../../../minterm.md)

$$
\chi_T=
\left(\bigwedge_{s_i\in T}x_i\right)\land
\left(\bigwedge_{s_i\notin T}\neg x_i\right).
$$

A [Boolean valuation](../../../../../boolean-valuation.md) satisfies $\chi_T$ exactly when its selected subset is $T$. Therefore the [weighted formula utility representation](../../../../../weighted-formula-utility-representation.md)

$$
\mathcal R_u=\{(\chi_T,u(T)):T\subseteq S\}
$$

represents $u$ exactly: at the [Boolean valuation](../../../../../boolean-valuation.md) for $T$, only that [minterm](../../../../../minterm.md) contributes, with weight $u(T)$. This proves **completeness and the bound of $2^{|S|}$ rules** simultaneously. Zero-weight rules may be omitted. The bound counts rules; writing each [minterm](../../../../../minterm.md) also requires $O(m)$ symbols in [Big O notation](../../../../../big-o-notation.md).

For the computational question, assume rule weights are [rational numbers](../../../../../rational-number.md) encoded in binary. This makes exact equality of sums a finite computational task. With this conventional encoding, **equivalence of [weighted formula utility representations](../../../../../weighted-formula-utility-representation.md) is [co-NP](../../../../../co-np.md)-complete**.

For membership, the complement has a short witness: a [Boolean valuation](../../../../../boolean-valuation.md) on the variables occurring in either rule base. Evaluate each [propositional formula](../../../../../propositional-formula.md), sum the weights of satisfied rules, and accept the witness if the sums differ. [Propositional formula](../../../../../propositional-formula.md) evaluation takes [polynomial time](../../../../../polynomial-time.md). Exact sums of binary [rational numbers](../../../../../rational-number.md) also have polynomially bounded bit lengths: the product of their denominators has bit length at most the sum of the input denominator lengths. Thus non-equivalence lies in [NP](../../../../../np-complexity.md), and equivalence lies in [co-NP](../../../../../co-np.md).

For hardness, take a [Boolean satisfiability problem](../../../../../boolean-satisfiability-problem.md) instance $\theta$ and construct

$$
\mathcal R_1=\{(\theta,1)\},\qquad \mathcal R_2=\varnothing.
$$

The first [utility function](../../../../../utility-function-split.md) is one at satisfying [Boolean valuations](../../../../../boolean-valuation.md) and zero elsewhere, while the second is always zero. Consequently

$$
\mathcal R_1\equiv\mathcal R_2
\iff \theta\text{ is an unsatisfiable Boolean formula}.
$$

The [unsatisfiable Boolean formula](../../../../../unsatisfiable-boolean-formula.md) problem is [co-NP](../../../../../co-np.md)-complete, as the complement of the [NP](../../../../../np-complexity.md)-complete [Boolean satisfiability problem](../../../../../boolean-satisfiability-problem.md). The construction is a [polynomial-time reduction](../../../../../polynomial-time-reduction.md), proving hardness even with the single weight $1$.

Two qualifications matter in the literal wording. First, unrestricted real weights have no specified finite encoding, so a standard bit-complexity classification needs the encoding assumption above. Second, the problem says only that $S$ is nonempty. If infinite $S$ is allowed while rule bases remain finite, its completeness claim is false. For $S=\mathbb N$, take $u(T)=1$ when $T$ is infinite and $u(T)=0$ when $T$ is finite. A finite rule base mentions only a finite subset $F$ of the variables. The [Boolean valuations](../../../../../boolean-valuation.md) for $\varnothing$ and $\mathbb N\setminus F$ agree on all those variables but have different required values. No such rule base represents this $u$. Thus the construction answers the intended finite-set question and identifies the missing hypothesis in the unrestricted statement.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2023](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
