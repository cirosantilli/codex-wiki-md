<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $s=R^2$. A steady [complex amplitude](../../../../../../complex-amplitude.md) obeys $(\mu-s+i\Lambda)A=-1$, so

$$
\boxed{A=\frac{s-\mu+i\Lambda}{(\mu-s)^2+\Lambda^2},\qquad s[(\mu-s)^2+\Lambda^2]=1.}
$$

Thus every positive intensity root gives exactly one steady phase, and $s=0$ is impossible. The cubic intensity [polynomial](../../../../../../polynomial-split.md) is $F(s,\mu)=s^3-2\mu s^2+(\mu^2+\Lambda^2)s-1$. Its positive steady branch can be parameterized completely as

$$
\mu_\pm(s)=s\pm\sqrt{s^{-1}-\Lambda^2},\qquad 0<s\leq\Lambda^{-2},\qquad R=\sqrt s.
$$

The two formulae join smoothly as a single curve at the maximum radius $R=\Lambda^{-1}$; this joining point is not a [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md). A turning point with respect to $\mu$ satisfies $F_s=0$. Subtracting the [equilibrium](../../../../../../equilibrium-point-of-a-dynamical-system.md) and [derivative](../../../../../../derivative.md) conditions gives

$$
\mu-s=\frac1{2s^2},\qquad
\boxed{\Lambda^2=f(s):=\frac1s-\frac1{4s^4},\qquad \mu=s+\frac1{2s^2}.}
$$

These points lie on $\mu_+$. Since $f'(s)=(1-s^3)/s^5$, its maximum is $f(1)=3/4$. Therefore **there is exactly one distinct steady state for every $\mu$ when $\Lambda\geq\sqrt3/2$**. One can also see uniqueness directly: $\mu_-$ is increasing and $\mu_+$ is decreasing when no turning points exist, and their respective ranges meet only at their common endpoint. At the equality there is a [cusp bifurcation](../../../../../../cusp-bifurcation.md) with a triple intensity root at $s=1,\mu=3/2$.

When $0<\Lambda<\sqrt3/2$, the two turning intensities satisfy $s_-<1<s_+$. Define $\mu_L=s_-+1/(2s_-^2)$ and $\mu_U=s_++1/(2s_+^2)$; the curve has a local minimum at the former and a local maximum at the latter, with $\mu_L<\mu_U$. There are three distinct steady intensities for $\mu_L<\mu<\mu_U$, two distinct ones at an endpoint, and one otherwise. The [bifurcation diagrams](../../../../../../bifurcation-diagram.md) below show the folded small-$\Lambda$ curves and the unfurled large-$\Lambda$ curve, together with the [linear stability](../../../../../../linear-stability.md) calculated next. Both ends of the full branch have $R\to0$ as $|\mu|\to\infty$, while its middle reaches the finite maximum $\Lambda^{-1}$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
