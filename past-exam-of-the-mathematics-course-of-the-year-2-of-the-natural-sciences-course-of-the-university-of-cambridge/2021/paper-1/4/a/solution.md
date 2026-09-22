<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First take a [Schwartz function](../../../../../schwartz-function.md), so that [Fourier inversion](../../../../../fourier-inversion-theorem.md) and the exchange of integrals are justified. Inserting the inverse transform of the [complex conjugate](../../../../../complex-conjugate.md) gives

$$
\begin{aligned}
\int_{\mathbb R}|f(x)|^2dx
&=\frac1{2\pi}\int_{\mathbb R}\!\int_{\mathbb R} f(x)\overline{\widetilde f(k)}e^{-ikx}\,dk\,dx\\
&=\frac1{2\pi}\int_{\mathbb R}\overline{\widetilde f(k)}\left[\int_{\mathbb R}f(x)e^{-ikx}dx\right]dk\\
&=\boxed{\frac1{2\pi}\int_{\mathbb R}|\widetilde f(k)|^2dk.}
\end{aligned}
$$

For $f\in L^1\cap L^2$, approximate it by [Schwartz functions](../../../../../schwartz-function.md) in both [norms](../../../../../norm.md). The identity just proved makes their transforms a [Cauchy sequence](../../../../../cauchy-sequence.md) in [L2 space](../../../../../l2-space-is-a-hilbert-space.md), while convergence in [L1 space](../../../../../l1-space.md) makes the transforms converge uniformly to the defining transform of $f$. Thus the two transform limits agree, and passing to the $L^2$ [norms](../../../../../norm.md) proves the finite [Parseval identity](../../../../../parseval-identity.md). This is the normalization of the [Plancherel theorem](../../../../../plancherel-theorem.md) appropriate to the paper.

There is a qualification to the printed hypothesis: absolute integrability alone does not guarantee a finite square integral. For instance $f(x)=x^{-3/4}$ on $(0,1)$ and zero elsewhere belongs to $L^1$ but not $L^2$. For an $L^1$ function of this kind the transform is not in $L^2$ either, by [L2 density from a square-integrable Fourier transform](../../../../../l2-density-from-a-square-integrable-fourier-transform.md), so both sides are infinite if the identity is interpreted in that extended sense. The finite equality requires square integrability as well.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
