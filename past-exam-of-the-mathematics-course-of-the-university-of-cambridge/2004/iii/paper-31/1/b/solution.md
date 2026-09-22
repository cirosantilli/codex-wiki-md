<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $m=\lceil(b-a)/\varepsilon\rceil$. The ceiling, as printed in the PDF, makes the intervals cover the bounded range of f. If $a=b$, use the single set $\mathcal X$ instead, since f is constant. By [continuity](../../../../../../continuous-function.md) their preimages are closed. On every nonempty preimage $C_i$, the oscillation of f is at most epsilon. Hence for every $y\in C_i$,

$$
\sup_{C_i}f\leq f(y)+\varepsilon,\qquad\sup_{C_i}f-I(y)\leq\sup_{x\in\mathcal X}(f(x)-I(x))+\varepsilon.
$$

Taking the [supremum](../../../../../../supremum.md) over y in the second expression gives the bound for $\sup_{C_i}f-\inf_{C_i}I$; if that [infimum](../../../../../../infimum.md) is infinite, the bound is automatic. Apply the finite-cover estimate to obtain

$$
\boxed{\limsup_n n^{-1}\log\mathbb E e^{nf(X_n)}\leq\sup_x(f(x)-I(x))+\varepsilon.}
$$

This is the exponential-integral upper estimate in the bounded form of [Varadhan lemma](../../../../../../varadhan-s-lemma.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
