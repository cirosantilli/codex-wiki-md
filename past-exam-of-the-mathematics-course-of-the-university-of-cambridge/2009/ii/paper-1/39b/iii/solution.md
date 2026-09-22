<h1 id="39b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a fixed $n$, convergence for every initial error is equivalent to $|1-\omega t_k|<1$ for all $k$, where $t_k=1-\cos(k\pi/(n+1))>0$. Thus

$$
0<\omega<\frac{2}{1+\cos(\pi/(n+1))}
=\frac1{\cos^2(\pi/[2(n+1)])}.
$$

A single parameter works for every finite $n$ precisely when **$\boxed{0<\omega\leq1}$**: the largest $t_k$ tends to two as $n\to\infty$, so every $\omega>1$ eventually fails, whereas $\omega=1$ has all [eigenvalues](../../../../../../eigenvalue.md) strictly between $-1$ and one for each finite grid.

For such $\omega$ the lowest-frequency [eigenvalue](../../../../../../eigenvalue.md) satisfies, using $1-\cos x\leq x^2/2$,

$$
\lambda_1(\omega)=1-\omega(1-\cos(\pi/(n+1)))
\geq1-\frac{\pi^2}{2(n+1)^2}.
$$

An initial error proportional to $v_1$ retains exactly the factor $\lambda_1^\nu$. Hence the worst-case [spectral radius](../../../../../../spectral-radius.md) cannot improve on a factor of the form **$(1-c/n^2)^\nu$**, with $c$ independent of grid size, and reducing a slow-mode error by a fixed fraction takes order $n^2$ iterations. This is a worst-case rate assertion, not a lower bound for every individual initial error: a vector containing only faster modes, or the zero vector, need not exhibit the slow mode.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [39B](../../39b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
