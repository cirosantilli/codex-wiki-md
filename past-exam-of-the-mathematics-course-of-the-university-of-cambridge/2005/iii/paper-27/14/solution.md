<h1 id="14/solution">Solution</h1>

↑ **Parent:** [14](../14.md)

Use [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) and infinite input sets, the usual scope of the stated claim. For a finite set of size $n$, its [Hartogs number](../../../../../hartogs-number.md) is $n+1$, which is a finite successor cardinal rather than an aleph. Without the [axiom of choice](../../../../../axiom-of-choice.md), one cannot silently identify every infinite input with an aleph, and the asserted conclusion needs those hypotheses.

The [Hartogs number](../../../../../hartogs-number.md) $h(X)$ is the least ordinal that does not inject into $X$. It is an [initial ordinal](../../../../../initial-ordinal.md): if it were equinumerous with a smaller ordinal $\alpha<h(X)$, composing that bijection with an injection $\alpha\to X$ would contradict its definition. With choice, well-order an infinite $X$ and put $|X|=\kappa=\aleph_\eta$. Every ordinal below $\kappa^+$ has cardinal at most $\kappa$ and injects into $X$, whereas $\kappa^+$ does not. Hence the [Hartogs numbers under choice](../../../../../hartogs-numbers-under-choice.md) satisfy

$$
\boxed{h(X)=\kappa^+=\aleph_{\eta+1}}.
$$

To prove regularity, suppose $\operatorname{cf}(\kappa^+)=\mu<\kappa^+$. Since $\kappa^+$ is a successor cardinal, $\mu\le\kappa$. Choose a cofinal sequence $\langle\alpha_i:i<\mu\rangle$ below $\kappa^+$. Each $\alpha_i$ has cardinal at most $\kappa$, and choice gives

$$
\left|\bigcup_{i<\mu}\alpha_i\right|\le\mu\cdot\kappa\le\kappa.
$$

But cofinality makes this union all of $\kappa^+$, a contradiction. Therefore $\operatorname{cf}(\kappa^+)=\kappa^+$, and every infinite-input Hartogs value is a regular initial successor aleph. Conversely every successor aleph occurs by taking $X$ to be its predecessor cardinal.

## ↑ Ancestors (10)

1. [14](../14.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
