<h1 id="2/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

The [Krivine rounding constant](../../../../../../krivine-rounding-constant.md) has $t=c_K\pi/2=\log(1+\sqrt2)<\pi/2$. Since $|X_{ij}|\leq1$, the principal real [inverse sine](../../../../../../inverse-sine.md) satisfies

$$
\arcsin(\sin(tX_{ij}))=tX_{ij}
$$

on every cross-block entry. The [matrix](../../../../../../matrix.md) $A$ has zero diagonal blocks, so those cross blocks are the only contributors to its [Frobenius inner product](../../../../../../frobenius-inner-product.md) with $\arcsin[Y]$. Explicitly,

$$
\operatorname{tr}(A\arcsin[Y])
=\sum_{i=1}^n\sum_{j=1}^mS_{ij}\arcsin(g(X_{i,n+j}))
=t\sum_{i,j}S_{ij}X_{i,n+j}
=t\operatorname{tr}(AX).
$$

No analogous identity is needed for the diagonal blocks involving $\sinh$.

Combining with the preceding [expectation](../../../../../../expected-value.md) formula and optimality of $X$ gives the [bipartite sign rounding bound](../../../../../../bipartite-sign-rounding-bound.md)

$$
\boxed{c_Kp_{\rm SDP}^*\leq v^*\leq p_{\rm SDP}^*},\qquad
\boxed{c_K=\frac2\pi\log(1+\sqrt2)=0.56109985\ldots}.
$$

At least one feasible rounded outcome attains at least this [expectation](../../../../../../expected-value.md). This is an expectation-based approximation guarantee for the specific bipartite sign problem; no claim is made that $c_K$ is the largest possible constant. The inequalities remain valid when the optimal objective is zero.

## ↑ Ancestors (11)

1. [G](../g.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
