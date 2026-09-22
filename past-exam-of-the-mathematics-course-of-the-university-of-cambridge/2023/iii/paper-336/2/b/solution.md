<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the summand as $a_n=x^n/[\Gamma(n)n^n]$. By [Stirling formula](../../../../../../stirling-formula.md),

$$
a_n\sim\frac{n^{1/2}}{\sqrt{2\pi}}
\exp\left[n(\log x+1-2\log n)\right].
$$

Set

$$
N=\sqrt{\frac xe},
\qquad n=Nt.
$$

Then the exponential phase is

$$
n(\log x+1-2\log n)
=Nf(t),
\qquad
f(t)=2t(1-\log t).
$$

It has a unique maximum at $t=1$, where $f(1)=2$ and $f''(1)=-2$. The contributing indices satisfy $n-N=O(\sqrt N)$, so their width tends to infinity and the lattice sum may be replaced by a [Riemann sum](../../../../../../riemann-sum.md). The [Discrete Laplace method](../../../../../../discrete-laplace-method.md) therefore gives

$$
S\sim
N\frac{\sqrt N}{\sqrt{2\pi}}e^{2N}
\sqrt{\frac{2\pi}{2N}}
=\frac{N}{\sqrt2}e^{2N}.
$$

Hence

$$
\boxed{
S\sim\sqrt{\frac{x}{2e}}
\exp\left(2\sqrt{\frac xe}\right)}
\qquad(x\to\infty).
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
