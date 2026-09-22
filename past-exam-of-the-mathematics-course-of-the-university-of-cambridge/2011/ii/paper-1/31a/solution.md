<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

The [asymptotic expansion](../../../../../asymptotic-expansion.md) means that for every fixed integer $M\geq0$,

$$
f(n)-\sum_{k=0}^Ma_kn^{-2k}=o(n^{-2M})\qquad(n\to\infty).
$$

It concerns the successive finite truncations; the infinite series need not converge. Because the assertion holds at every order, one may equivalently bound the remainder after order $M$ by $O(n^{-2M-2})$.

Put $h(t)=(1+t^2)^{-1}$ and $b=2\pi$. For integer $n$, $\sin(nb)=\sin0=0$ and $\cos(nb)=\cos0=1$. Two [integrations by parts](../../../../../integration-by-parts.md) give

$$
I(n)=\frac{h'(b)-h'(0)}{n^2}-\frac1{n^2}\int_0^bh''(t)\cos(nt)\,dt.
$$

Repeating exactly $M$ times gives

$$
I(n)=\sum_{k=1}^M\frac{(-1)^{k-1}[h^{(2k-1)}(b)-h^{(2k-1)}(0)]}{n^{2k}}+\frac{(-1)^M}{n^{2M}}\int_0^bh^{(2M)}(t)\cos(nt)\,dt.
$$

All derivatives are integrable on this compact interval. The [Riemann-Lebesgue lemma](../../../../../riemann-lebesgue-lemma.md) says their oscillatory integrals tend to zero, proving the expansion at every order, including $a_0=0$. Since $h$ is even, its odd derivatives vanish at zero. Now $h'(t)=-2t/(1+t^2)^2$ and $h'''(t)=24t(1-t^2)/(1+t^2)^4$, so

$$
\boxed{a_0=0,\qquad a_1=-\frac{4\pi}{(1+4\pi^2)^2},\qquad a_2=\frac{48\pi(4\pi^2-1)}{(1+4\pi^2)^4}.}
$$

The restriction to integer $n$ is essential to this even-power endpoint expansion: otherwise the first integration by parts has a generally nonzero $n^{-1}$ boundary term.

## ↑ Ancestors (11)

1. [31A](../31a.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
