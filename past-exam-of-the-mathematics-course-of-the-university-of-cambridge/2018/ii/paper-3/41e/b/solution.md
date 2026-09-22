<h1 id="41e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [discrete Fourier mode](../../../../../../discrete-fourier-mode.md) $u_m^n=r^ne^{im\theta}$, put

$$
q=4\mu\sin^2\frac\theta2,
\qquad 0\leq q\leq4\mu.
$$

The recurrence becomes

$$
r^{n+1}=\left(1-\frac32q\right)r^n+\frac12qr^{n-1},
$$

so its [amplification polynomial of a multilevel finite difference scheme](../../../../../../amplification-polynomial-of-a-multilevel-finite-difference-scheme.md) is

$$
p(r)=r^2-\left(1-\frac32q\right)r-\frac12q.
$$

Its roots are real. Moreover,

$$
p(1)=q,
\qquad
p(-1)=2(1-q),
\qquad
\frac{r_1+r_2}{2}=\frac12-\frac34q.
$$

The root-location criterion in the question therefore puts both roots in $[-1,1]$ exactly when $0\leq q\leq1$. [Fourier stability analysis](../../../../../../fourier-stability-analysis.md) for every [wavenumber](../../../../../../wavenumber.md) is equivalent to $4\mu\leq1$, so

$$
\boxed{\text{the scheme is stable if and only if }\mu\leq\frac14.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [41E](../../41e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
