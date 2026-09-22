<h1 id="14e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

If $\operatorname{Im}z>0$, the same upper-half-plane contour calculation gives

$$
G(z)=\frac{2\pi i^ne^{iz}}{(n-1)!}.
$$

If $\operatorname{Im}z<0$, the pole lies below the real integration contour. Closing upward encloses no pole, so [Jordan lemma](../../../../../../jordan-s-lemma.md) and the [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) give

$$
G(z)=0.
$$

Hence at a real point $x$ the upper and lower boundary values satisfy

$$
\boxed{
G(x+i0)-G(x-i0)
=\frac{2\pi i^ne^{ix}}{(n-1)!}
}.
$$

Thus crossing from the upper half-plane to the lower half-plane produces the negative of this jump.

An [analytic continuation](../../../../../../analytic-continuation.md) must be holomorphic, hence [continuous](../../../../../../continuous-function.md), across every point where it is defined. The undeformed real-axis formula for $G$ has the nonzero jump above, while the continuation constructed in part (c) retains $2\pi i^ne^{iz}/(n-1)!$ below the axis. Therefore $G$ cannot be the analytic continuation of $F$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
