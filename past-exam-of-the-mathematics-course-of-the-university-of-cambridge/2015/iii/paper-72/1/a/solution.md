<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\epsilon>0$, [dominant balance for algebraic roots](../../../../../../dominant-balance-for-algebraic-roots.md) gives two roots on the scale $\sqrt\epsilon$ and a third on the scale $\epsilon^{2/3}$. On the first scale put $t=\sqrt\epsilon\,s$. The equation becomes $s^5-s^3+\sqrt\epsilon=0$. The [derivative](../../../../../../derivative.md) of $s^5-s^3$ at either $s=1$ or $s=-1$ is two, so the first correction is $-\sqrt\epsilon/2$. On the second scale put $t=\epsilon^{2/3}v$; then $1-v^3+\epsilon^{1/3}v^5=0$. Writing $v=1+a\epsilon^{1/3}+\cdots$ gives $a=1/3$. Thus **all three real-root expansions for positive $\epsilon$ are**

$$
\boxed{t_\pm=\pm\epsilon^{1/2}-\tfrac12\epsilon+O(\epsilon^{3/2}),\qquad
t_0=\epsilon^{2/3}+\tfrac13\epsilon+O(\epsilon^{4/3}).}
$$

These are [fractional-power root expansions](../../../../../../fractional-power-root-expansion.md). To check that none is missing, the [derivative](../../../../../../derivative.md) of the [polynomial](../../../../../../polynomial-split.md) is $t^2(5t^2-3\epsilon)$. Its nonzero [critical points](../../../../../../critical-point.md) are $\pm\sqrt{3\epsilon/5}$; for sufficiently small positive $\epsilon$ the [polynomial](../../../../../../polynomial-split.md) is positive at the negative one and negative at the positive one. Its three monotone ranges therefore contain exactly these three real roots. The remaining two small roots correspond to the nonreal cube roots of unity in the second balance.

The printed limit does not specify the sign of $\epsilon$. If a two-sided real limit is intended, also put $\epsilon=-\eta$ with $\eta>0$. The [polynomial](../../../../../../polynomial-split.md) $t^5+\eta t^3-\eta^3$ is strictly increasing and has just one real root. The same [dominant balance for algebraic roots](../../../../../../dominant-balance-for-algebraic-roots.md) gives **the negative-parameter branch**

$$
\boxed{t=\eta^{2/3}-\tfrac13\eta+O(\eta^{4/3}),\qquad\eta=-\epsilon\downarrow0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
