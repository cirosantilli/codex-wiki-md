<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

A straight [quantum vortex](../../../../../../quantum-vortex.md) with integer [winding number](../../../../../../winding-number.md) $\mathcal N$ has $\widetilde\psi=R(r)e^{i\mathcal N\theta}$, independent of $z$. Here $r$ is measured in the unit of distance from the preceding part. The polar [Laplacian](../../../../../../laplacian.md) supplies the centrifugal term, giving

$$
\boxed{R''+\frac{R'}r-\frac{\mathcal N^2}{r^2}R
+(1-\alpha R^2-\beta R^4)R=0}.
$$

For $\mathcal N\ne0$, regularity requires $R\sim c r^{|\mathcal N|}$ near the axis; the bulk condition is $R\to1$. The full [wavefunction](../../../../../../wave-function.md) tends to $e^{i\mathcal N\theta}$ rather than one. This is the [constant far-field phase excludes net vortex winding](../../../../../../constant-far-field-phase-excludes-net-vortex-winding.md) distinction: the equation remains applicable to a vortex, but the nonwinding boundary condition must be interpreted as an amplitude condition.

Let $F(R)=R-\alpha R^3-\beta R^5$. Since $\alpha+\beta=1$, one has $F(1)=0$ and $F'(1)=1-3\alpha-5\beta=-2(1+\beta)$. Insert $R=1-p/r^2+\cdots$. Its derivative terms start at order $r^{-4}$, while

$$
-\frac{\mathcal N^2R}{r^2}=-\frac{\mathcal N^2}{r^2}+O(r^{-4}),\qquad
F(R)=\frac{2(1+\beta)p}{r^2}+O(r^{-4}).
$$

Cancellation of the order-$r^{-2}$ terms proves the [cubic-quintic quantum vortex tail](../../../../../../cubic-quintic-quantum-vortex-tail.md)

$$
\boxed{R(r)=1-\frac{\mathcal N^2}{2(1+\beta)r^2}+O(r^{-3}),\qquad
p=\frac{\mathcal N^2}{2(1+\beta)}}.
$$

For a stable nondegenerate bulk state in this scaling, $1+\beta=n_0(V_0+2W_0n_0)/\mu>0$. At $\beta=-1$ the amplitude restoring derivative vanishes, and an inverse-square perturbation cannot cancel the centrifugal term, so the stated expansion fails. For zero winding the uniform solution has $p=0$.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
