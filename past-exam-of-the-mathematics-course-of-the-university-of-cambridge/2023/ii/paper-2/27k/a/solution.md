<h1 id="27k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the convention

$$
\widehat f(u)=\int_{\mathbb R^d}e^{iu\cdot x}f(x)\,dx.
$$

The [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) says that, when $f,\widehat f\in L^1(\mathbb R^d)$,

$$
f(x)=\frac1{(2\pi)^d}
\int_{\mathbb R^d}e^{-iu\cdot x}\widehat f(u)\,du
$$

for almost every $x$.

Since

$$
\overline{\widehat f(u)}
=\int_{\mathbb R^d}e^{-iu\cdot x}\overline{f(x)}\,dx,
$$

the [Fubini's theorem](../../../../../../fubini-s-theorem.md) and Fourier inversion give

$$
\begin{aligned}
\int_{\mathbb R^d}|\widehat f(u)|^2\,du
&=\int_{\mathbb R^d}\widehat f(u)
 \int_{\mathbb R^d}e^{-iu\cdot x}\overline{f(x)}\,dx\,du\\
&=\int_{\mathbb R^d}\overline{f(x)}
 \int_{\mathbb R^d}e^{-iu\cdot x}\widehat f(u)\,du\,dx\\
&=(2\pi)^d\int_{\mathbb R^d}|f(x)|^2\,dx.
\end{aligned}
$$

Thus the [Plancherel theorem](../../../../../../plancherel-theorem.md) identity in this convention is

$$
\boxed{\|\widehat f\|_2^2=(2\pi)^d\|f\|_2^2.}
$$

The inverse integral is a continuous function of $x$, since $\widehat f\in L^1$ permits dominated convergence. If $f$ is continuous, it and the inverse integral are continuous and agree almost everywhere. They must agree everywhere: otherwise their continuous difference would be nonzero on an open set of positive measure. This is the [continuous version of Fourier inversion](../../../../../../continuous-version-of-fourier-inversion.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27K](../../27k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
