<h1 id="31e/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

To obtain a [basin estimate from a Lyapunov sublevel set](../../../../../../../basin-estimate-from-a-lyapunov-sublevel-set.md), take the largest sublevel component around the origin that remains inside the strict-decrease rectangle. On its boundary $|x|=\sqrt2$ or $|y|=\pi/2$, the minimum value of $V$ is $1$. Hence the maximal open estimate is

$$
\boxed{
\mathcal D_V=
\left\{(x,y): |y|<\frac\pi2,
\ \frac{x^2}{2}+\sin^2y<1\right\}}.
$$

Every smaller closed sublevel set $V\leq c<1$ is compact and positively invariant, and $\dot V<0$ there except at the origin. The [LaSalle invariance principle](../../../../../../../lasalle-s-invariance-principle.md) therefore implies convergence to the origin. Taking the union over $c<1$ shows that $\mathcal D_V$ lies in the domain of stability. No larger sublevel component can be certified from this $V$ alone, because every level $c>1$ contains points $(0,y)$ just beyond $|y|=\pi/2$ where $\dot V>0$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [31E](../../../31e.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
