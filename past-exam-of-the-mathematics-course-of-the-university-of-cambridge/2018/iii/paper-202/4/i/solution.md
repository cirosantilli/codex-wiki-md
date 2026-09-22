<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the standard definition of a [local martingale](../../../../../../local-martingale.md), including an integrable initial value, and let $T_n\uparrow\infty$ be a [localizing sequence](../../../../../../localizing-sequence.md). If $X\geq0$, the [Fatou lemma](../../../../../../fatou-s-lemma.md) gives $\mathbb EX_t\leq\liminf_n\mathbb EX_{t\wedge T_n}=\mathbb EX_0<\infty$. For $s\leq t$, the [Conditional Fatou lemma](../../../../../../conditional-fatou-lemma.md) gives

$$
\mathbb E(X_t\mid\mathcal F_s)\leq\liminf_n\mathbb E(X_{t\wedge T_n}\mid\mathcal F_s)=\liminf_nX_{s\wedge T_n}=X_s.
$$

For clarity, the [Conditional Fatou lemma](../../../../../../conditional-fatou-lemma.md) itself follows by setting $U_m=\inf_{n\geq m}U_n$ for nonnegative $U_n$, applying the conditional version of the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) to $U_m\uparrow\liminf U_n$, and observing $\mathbb E(U_m\mid\mathcal F_s)\leq\inf_{n\geq m}\mathbb E(U_n\mid\mathcal F_s)$. Hence **a nonnegative [local martingale](../../../../../../local-martingale.md) is a [supermartingale](../../../../../../supermartingale.md).**

If $|X_t|\leq C$ simultaneously for all $t$, with a deterministic $C<\infty$, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) applied to the stopped [martingale](../../../../../../martingale-split.md) identity gives, for each $A\in\mathcal F_s$,

$$
\mathbb E(\mathbf1_AX_t)=\lim_n\mathbb E(\mathbf1_AX_{t\wedge T_n})=\lim_n\mathbb E(\mathbf1_AX_{s\wedge T_n})=\mathbb E(\mathbf1_AX_s).
$$

This is exactly the [conditional expectation](../../../../../../conditional-expectation.md) identity, so **a bounded [local martingale](../../../../../../local-martingale.md) is a true [martingale](../../../../../../martingale-split.md).** The same proof works for deterministic bounds on every finite time interval; merely having a finite random pathwise bound supplies no dominating integrable [random variable](../../../../../../random-variable-split.md) and is a different convention.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
