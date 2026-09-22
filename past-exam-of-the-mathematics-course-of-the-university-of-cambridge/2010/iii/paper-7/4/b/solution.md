<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every entire [holomorphic function](../../../../../../holomorphic-function.md) has a [Taylor series](../../../../../../taylor-series.md) $f(z)=\sum_{n\geq0}a_nz^n$, uniformly convergent on each circle. Angular [orthogonality](../../../../../../orthogonal-vectors.md) gives

$$
\frac1{2\pi}\int_0^{2\pi}|f(re^{i\theta})|^2\,d\theta=\sum_{n\geq0}|a_n|^2r^{2n}.
$$

Integrate in polar coordinates and use [Tonelli theorem](../../../../../../tonelli-theorem.md) for the nonnegative sum:

$$
\|f\|_{\mathcal F}^2
=2\sum_{n\geq0}|a_n|^2\int_0^\infty r^{2n+1}e^{-r^2}\,dr
=\sum_{n\geq0}n!|a_n|^2.
$$

The last integral equals $n!/2$ by substituting $u=r^2$ and repeated [integration by parts](../../../../../../integration-by-parts.md).

Conversely, for any $(b_n)\in\ell^2$, set $a_n=b_n/\sqrt{n!}$. On $|z|\leq R$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_{n\geq0}|a_nz^n|
\leq\left(\sum_n|b_n|^2\right)^{1/2}\left(\sum_n\frac{R^{2n}}{n!}\right)^{1/2}
=\|(b_n)\|_{\ell^2}e^{R^2/2}.
$$

Applied to the tails, the same bound proves uniform convergence on every disk. The series therefore defines an entire [holomorphic function](../../../../../../holomorphic-function.md), and the norm identity puts it in the [Bargmann-Fock space](../../../../../../bargmann-fock-space.md) $\mathcal F$. The coefficient map $f\mapsto(\sqrt{n!}a_n)$ is consequently an onto linear isometry $\mathcal F\to\ell^2$; polarization also identifies the inner products. Completeness of $\ell^2$ proves that $\mathcal F$ is a [Hilbert space](../../../../../../hilbert-space-split.md). Its standard coordinate [orthonormal basis](../../../../../../orthonormal-basis.md) corresponds to

$$
\boxed{e_n(z)=\frac{z^n}{\sqrt{n!}},\quad n=0,1,\ldots.}
$$

The norm identity shows both their unit norms and completeness; it also gives $|f(z)|\leq e^{|z|^2/2}\|f\|_{\mathcal F}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
