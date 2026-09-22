<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Apply the [direct method in the calculus of variations](../../../../../../direct-method-in-the-calculus-of-variations.md) to $J(u)=\|f-Ku\|_1+\alpha|Du|(\Omega)$. Since $J(0)=\|f\|_1$, take a [minimizing sequence](../../../../../../minimizing-sequence.md) with $J(u_k)\le C:=\|f\|_1+1$. Then

$$
|Du_k|(\Omega)\le C/\alpha,\qquad \|Ku_k\|_1\le\|f\|_1+C,\qquad \|u_k\|_1\le\|K^{-1}\|\,(\|f\|_1+C).
$$

Thus the sequence is bounded in the [bounded-variation space](../../../../../../function-of-bounded-variation-on-a-domain.md). The [bounded-variation compactness](../../../../../../bounded-variation-compactness.md) gives a [subsequence](../../../../../../subsequence.md) converging in the [strong convergence](../../../../../../norm-convergence.md) sense in $L^1$ to $u\in BV(\Omega)$. Boundedness of the [linear operator](../../../../../../linear-operator.md) $K$ gives $Ku_k\to Ku$ strongly in $L^1$, so the residual [norm](../../../../../../norm.md) converges. The variation term is [sequentially lower semicontinuous](../../../../../../sequential-lower-semicontinuity.md), hence

$$
\boxed{J(u)\le\liminf_kJ(u_k)=\inf_{v\in BV(\Omega)}J(v).}
$$

Therefore $u$ attains the infimum. The useful inverse hypothesis is the lower bound $\|u\|_1\le C_K\|Ku\|_1$; a [bounded inverse](../../../../../../bounded-inverse.md) on the range already suffices for this proof. No uniqueness follows from the nonsquared $L^1$ fidelity.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
