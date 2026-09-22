<h1 id="15g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $y=e^{-x/2}v$, the [Dirichlet gauge transform for constant drift](../../../../../../dirichlet-gauge-transform-for-constant-drift.md). Direct differentiation gives

$$
y''+y'=e^{-x/2}(v''-v/4).
$$

The homogeneous endpoint conditions on $y$ become $v(0)=v(1)=0$. Thus the eigenvalue equation is $v''=(\lambda+1/4)v$. To exclude other branches without assuming the eigenvalue real, multiply by $\bar v$ and integrate by parts:

$$
(\lambda+1/4)\int_0^1|v|^2\,dx=-\int_0^1|v'|^2\,dx<0
$$

for a nonzero [eigenfunction](../../../../../../eigenfunction.md). Therefore $\lambda+1/4=-k^2$ with $k>0$. The boundary conditions in $v=A\sin(kx)+B\cos(kx)$ give $B=0$ and $k=n\pi$, $n\ge1$. Hence

$$
\boxed{\lambda_n=-n^2\pi^2-\frac14,\qquad y_n(x)=e^{-x/2}\sin(n\pi x).}
$$

Equivalently, $L[y]=\lambda y$ is the [Sturm-Liouville form](../../../../../../sturm-liouville-form.md) $(e^xy')'=\lambda e^xy$, with positive weight $e^x$. Its [orthogonality](../../../../../../orthogonal-vectors.md) relation is

$$
\boxed{\int_0^1e^x y_m(x)y_n(x)\,dx=\frac12\delta_{mn}.}
$$

It is the weighted inner product, not the unweighted one, that makes these [eigenfunctions](../../../../../../eigenfunction.md) orthogonal.

Expand $xe^{-x/2}=\sum_nb_ny_n$ with the coefficients from part a. Completeness and the nonzero [eigenvalues](../../../../../../eigenvalue.md) give the [Sturm-Liouville eigenfunction expansion](../../../../../../sturm-liouville-eigenfunction-expansion.md)

$$
\boxed{y(x)=-e^{-x/2}\sum_{n=1}^{\infty}
\frac{2(-1)^{n+1}}{n\pi(n^2\pi^2+1/4)}\sin(n\pi x).}
$$

The coefficients are $O(n^{-3})$, so the function series converges uniformly and vanishes at both endpoints. Its first derivative also converges uniformly. Applying the transformed operator in the square-integrable sense gives the part-a expansion of $x$; equivalently $v''-v/4=x$ on the interior. Integrating this continuous right-hand side gives the classical twice-differentiable solution there. No nonzero homogeneous solution satisfies both endpoints, so this solution is unique. The mismatch of the forcing's sine series at a single endpoint does not affect the interior equation or these boundary conditions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15G](../../15g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
