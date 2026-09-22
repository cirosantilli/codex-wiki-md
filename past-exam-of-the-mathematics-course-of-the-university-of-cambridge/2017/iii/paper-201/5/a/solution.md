<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\tau_r=\inf\{t\geq0:|B_t|=r\}$, $\tau_R=\inf\{t\geq0:|B_t|=R\}$, and $\tau=\tau_r\wedge\tau_R$. The function $u(y)=|y|^{-1}$ is harmonic away from the origin: its [radial Laplacian](../../../../../../radial-laplacian.md) in dimension three is

$$
u''(\rho)+\frac2\rho u'(\rho)=\frac2{\rho^3}-\frac2{\rho^3}=0.
$$

The [Itô formula](../../../../../../ito-s-lemma.md) therefore makes $u(B_{t\wedge\tau})$ a [local martingale](../../../../../../local-martingale.md), bounded between $1/R$ and $1/r$, hence a true [martingale](../../../../../../martingale-split.md). The annulus exit time is finite [almost surely](../../../../../../almost-sure-convergence.md). For instance, exit from the containing [open ball](../../../../../../open-ball.md) is finite because from every point in the [open ball](../../../../../../open-ball.md) a sufficiently large [Gaussian vector](../../../../../../gaussian-random-vector.md) increment has a uniform positive probability of leaving it in unit time; iterate the [geometric tail bound from a uniform escape probability](../../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md).

The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at $t\wedge\tau$, followed by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), gives $\mathbb Eu(B_\tau)=u(x)$. By continuity, there is no radial overshoot and the two exit [spheres](../../../../../../sphere.md) cannot be hit simultaneously. Writing $p=\mathbb P_x(\tau_r<\tau_R)$ gives

$$
\frac1{|x|}=\frac pr+\frac{1-p}{R},\qquad
\boxed{p=\frac{|x|^{-1}-R^{-1}}{r^{-1}-R^{-1}}.}
$$

All harmonicity and boundedness statements apply only in the annulus, which stays away from the singularity at zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
