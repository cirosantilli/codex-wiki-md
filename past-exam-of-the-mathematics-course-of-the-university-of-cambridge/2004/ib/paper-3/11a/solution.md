<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

Let $B$ denote the zero-diagonal matrix with off-diagonal entries appearing in the iteration, and $G=-B/\alpha$ its [iteration matrix](../../../../../iteration-matrix.md). Its row sums are three, so $B\mathbf1=3\mathbf1$. The other eigenvalues are $2\omega+\omega^2$ and $2\omega^2+\omega$, where $\omega=e^{2\pi i/3}$, namely $-3/2\pm i\sqrt3/2$, both of modulus $\sqrt3$. Thus the [spectral radius](../../../../../spectral-radius.md) is $\rho(G)=3/|\alpha|$.

For $|\alpha|>3$, the infinity-norm estimate $\|G\|_\infty=3/|\alpha|<1$ already gives a contraction, so the iterates converge from every initial vector to the unique solution of $(\alpha I+B)x=b$. Conversely, two iterates whose initial difference is a nonzero multiple of $\mathbf1$ retain the difference $(-3/\alpha)^k\mathbf1$. This fails to decay when $|\alpha|\le3$, so convergence cannot be guaranteed for arbitrary starts. Therefore

$$
\boxed{|\alpha|>3.}
$$

At $\alpha=3$ the offending mode oscillates; at $\alpha=-3$ it is stationary and the coefficient matrix is singular. A specially chosen starting vector can suppress a bad mode, but that is not guaranteed convergence.

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
