<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Multiplication by $x^2$ puts the [eigenvalue problem](../../../../eigenvalue-problem.md) into [Sturm-Liouville form](../../../../sturm-liouville-form.md), $-(x^2y')'=\lambda x^2y$, with weight $x^2$. If $u,v$ correspond to distinct [eigenvalues](../../../../eigenvalue.md) $\lambda,\mu$, subtract their multiplied equations and integrate to get

$$
(\lambda-\mu)\int_0^\pi x^2uv\,dx=\left[x^2(uv'-vu')\right]_0^\pi=0.
$$

The upper boundary term vanishes by the [Dirichlet boundary condition](../../../../dirichlet-boundary-condition.md). For a bounded solution near zero, $x^2y'$ has a limit because $(x^2y')'=-\lambda x^2y$ is integrable. A nonzero limit would force a $1/x$ divergence in $y$, so that limit is zero; integration then gives $y'=O(x)$. The lower boundary term therefore also vanishes, proving the weighted [orthogonality](../../../../orthogonal-vectors.md).

Set $z=xy$. For $x>0$, $y''+2y'/x=z''/x$, and finiteness of $y(0)$ gives $z(0)=0$. Thus $z''+\lambda z=0$ with zero values at zero and $\pi$. The [radial Dirichlet spectrum in three dimensions](../../../../radial-dirichlet-spectrum-in-three-dimensions.md) gives

$$
\boxed{\lambda_n=n^2,\qquad y_n(x)=\frac{\sin nx}{x},\qquad n=1,2,\ldots,\quad y_n(0)=n.}
$$

The zero and negative [eigenvalues](../../../../eigenvalue.md) yield only the zero solution under these [boundary conditions](../../../../boundary-condition.md). Also $\int_0^\pi x^2y_n^2dx=\pi/2$.

For the forced equation, the same substitution gives $z''-\beta z=x$. The [Fourier sine series](../../../../fourier-sine-series.md) of $x$ on $(0,\pi)$ has coefficients

$$
b_n=\frac2\pi\int_0^\pi x\sin nx\,dx=\frac{2(-1)^{n+1}}n.
$$

Expanding $z=\sum c_n\sin nx$ gives $-(n^2+\beta)c_n=b_n$, hence

$$
\boxed{y(x)=2\sum_{n=1}^\infty\frac{(-1)^n}{n(n^2+\beta)}\frac{\sin nx}{x}.}
$$

The value at zero is defined by a [limit](../../../../limit-of-a-function.md). In fact $|\sin nx/x|\leq n$, so [uniform convergence](../../../../uniform-convergence.md) holds even there, by comparison with $2\sum(n^2+\beta)^{-1}$. An independent check comes from solving the constant-coefficient equation directly:

$$
y(x)=-\frac1\beta+\frac{\pi\sinh(\sqrt\beta x)}{\beta x\sinh(\pi\sqrt\beta)}.
$$

It satisfies both endpoint conditions and the forcing for $x>0$, and its finite origin limit agrees with the series. For $\beta>0$ the homogeneous boundary value problem has no nonzero solution, so the solution is unique.

## ↑ Ancestors (12)

1. [7](../7.md)
2. [Paper 1](../../paper-1-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
