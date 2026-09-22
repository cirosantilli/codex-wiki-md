<h1 id="31e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppress $(x,t)$, put $R(k)=b(k)/a(k)$ and $C=c e^{-2px+8p^3t}N(ip)$. Removing the pole gives the additive jump

$$
\mathcal M(k)-N(-k)=R(k)e^{2ikx+8ik^3t}N(k)-\frac C{k-ip}\equiv G(k),\qquad k\in\mathbb R.
$$

The upper analytic function is $\mathcal M-1$ and the lower analytic function is $N(-k)-1$. The [Cauchy integral formula](../../../../../../cauchy-integral-formula.md) and the [Sokhotski–Plemelj formula](../../../../../../sokhotski-plemelj-theorem.md) solve this jump as the upper and lower boundary values of $(2\pi i)^{-1}\int_\mathbb R G(s)/(s-z)\,ds$. At the lower point $z=-k$, with $\Im k>0$, this gives $N(k)-1$.

The rational part can be evaluated by closing the contour upward: $\int_\mathbb R[(s-ip)(s+k)]^{-1}ds=2\pi i/(k+ip)$. Thus the required linear integral equation is

$$
\boxed{N(k)=1-\frac{c e^{-2px+8p^3t}N(ip)}{k+ip}+\frac1{2\pi i}\int_\mathbb R\frac{R(s)e^{2isx+8is^3t}N(s)}{s+k}\,ds.}
$$

It is supplemented by its value at $k=ip$, and follows under the usual decay or principal-value hypotheses of the stated [Riemann-Hilbert problem](../../../../../../riemann-hilbert-problem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31E](../../31e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
