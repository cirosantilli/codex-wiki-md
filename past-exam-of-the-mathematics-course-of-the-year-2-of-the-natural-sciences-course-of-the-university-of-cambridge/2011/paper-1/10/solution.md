<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Use a [Lagrange multiplier](../../../../lagrange-multiplier.md) $\mu$ for the norm constraint. For real variations $u+\delta\eta$ with $\eta(0)=\eta(\pi)=0$, [integration by parts](../../../../integration-by-parts.md) gives

$$
\begin{aligned}
\delta(F-\mu G)&=2\int_0^\pi[u'\eta'+(\epsilon x-\mu)u\eta]dx\\
&=2\int_0^\pi[-u''+(\epsilon x-\mu)u]\eta\,dx.
\end{aligned}
$$

Thus stationarity is equivalent to the [Sturm-Liouville problem](../../../../sturm-liouville-problem.md)

$$
-u''+\epsilon xu=\mu u,\qquad u(0)=u(\pi)=0.
$$

Multiplying by $u$ and integrating shows $F[u]=\mu G[u]=\mu$, so the constrained stationary values are the [eigenvalues](../../../../eigenvalue.md), and the normalized stationary functions are their [eigenfunctions](../../../../eigenfunction.md). Conversely the eigenvalue equation makes the constrained first variation vanish. The [self-adjoint operator](../../../../self-adjoint-operator.md) has weight one.

For $\epsilon=0$, zero and negative eigenvalues yield no nonzero solution with both [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md). Positive eigenvalues have solutions $u=A\sin(\sqrt\lambda x)$ after the left condition, and the right condition gives $\sqrt\lambda=n$, $n\geq1$. Hence the lowest eigenpair is

$$
\boxed{\lambda_0=1,\qquad Y_1(x)=\sqrt{\frac2\pi}\sin x,}
$$

where the amplitude follows from $\int_0^\pi\sin^2x\,dx=\pi/2$.

The [Rayleigh-Ritz variational principle](../../../../rayleigh-ritz-variational-principle.md) bounds the full lowest eigenvalue by $F[Y_1]$. Its derivative contribution is one. For the linear potential, reflection about $\pi/2$ gives

$$
\int_0^\pi x\sin^2x\,dx=\frac\pi2\int_0^\pi\sin^2x\,dx=\frac{\pi^2}{4}.
$$

Thus the [sine trial bound for a linear potential on an interval](../../../../sine-trial-bound-for-a-linear-potential-on-an-interval.md) is

$$
\boxed{\lambda_\epsilon\leq1+\frac{\epsilon\pi}{2}.}
$$

For $\epsilon>0$ the bound is strict, since $-Y_1''+\epsilon xY_1=(1+\epsilon x)Y_1$ is not a constant multiple of $Y_1$. Also $\lambda_\epsilon\geq1$ by the [Poincaré inequality](../../../../poincare-inequality.md) and the nonnegative potential. Equality in the upper bound holds at $\epsilon=0$.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 1](../../paper-1-split.md)
3. [2011](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
