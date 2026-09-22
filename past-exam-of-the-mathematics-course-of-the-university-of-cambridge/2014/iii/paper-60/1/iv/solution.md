<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For each $x$, choose purifications $|u_x\rangle$ of $\rho_x$ and $|v_x\rangle$ of $\sigma_x$ in a common reference space. By [Uhlmann's theorem](../../../../../../uhlmann-s-theorem.md), the second can be chosen, including its overall phase, so that

$$
\langle u_x|v_x\rangle=F(\rho_x,\sigma_x)\geq0.
$$

Construct the two [flagged purifications of a quantum ensemble](../../../../../../flagged-purification-of-a-quantum-ensemble.md)

$$
|U\rangle=\sum_x\sqrt{p_x}|u_x\rangle|x\rangle,\qquad
|V\rangle=\sum_x\sqrt{p_x}|v_x\rangle|x\rangle.
$$

Their reduced states are the respective mixtures, and orthogonality of the flags gives $\langle U|V\rangle=\sum_xp_xF(\rho_x,\sigma_x)$. A particular purification overlap cannot exceed the maximizing overlap in [Uhlmann's theorem](../../../../../../uhlmann-s-theorem.md). Hence

$$
\boxed{F\left(\sum_xp_x\rho_x,\sum_xp_x\sigma_x\right)\geq\sum_xp_xF(\rho_x,\sigma_x).}
$$

This proves [joint concavity of quantum fidelity](../../../../../../joint-concavity-of-quantum-fidelity.md). Choosing each overlap nonnegative prevents cancellation of different phases; the same probability weights in the two mixtures yield $p_x$ rather than distinct square-root weights.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
