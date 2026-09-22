<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the observer have cylindrical coordinates $(r,\theta,z)$ and total distance $R=\sqrt{r^2+z^2}$. At retarded emission time $\tau$, the source-observer distance is

$$
|\mathbf x-\mathbf y(\tau)|=R-\frac{ar}{R}\cos(\Omega\tau-\theta)+O(a^2/R).
$$

The [retarded time](../../../../../../retarded-time.md) relation $t=\tau+|\mathbf x-\mathbf y(\tau)|/c_0$ consequently becomes

$$
\Omega\tau=\Omega(t-R/c_0)+m\cos(\Omega\tau-\theta),
\qquad m=\frac{\Omega ar}{c_0R}.
$$

Set $\Omega\tau=\theta-\pi/2+\Theta$. Then

$$
\boxed{\theta-\frac\pi2+\Theta=\Omega(t-R/c_0)+m\sin\Theta,}
\qquad
\dot\Theta=\frac{\Omega}{1-m\cos\Theta}.
$$

The observer-direction [Mach number](../../../../../../mach-number.md) at emission is $M_r=\dot{\mathbf y}(\tau)\cdot\mathbf n/c_0=m\cos\Theta$. For a constant strength $q$ and $m<1$, the single retarded root has $1-M_r>0$. Substituting into the moving-source field gives the [rotating acoustic point source](../../../../../../rotating-acoustic-point-source.md) result

$$
\boxed{\rho'(\mathbf x,t)=\frac{q}{4\pi c_0^2\Omega R}\frac{d\Theta}{dt}.}
$$

In particular, on the rotation axis $m=0$ and the result is $q/(4\pi c_0^2R)$.

For a genuinely varying source strength, replace $q$ by $q(\tau)$ in the last formula. If $m>1$, the retarded relation need not be one-to-one: each retarded root contributes with $|1-M_r|$ in the denominator. The general result is a sum of $q(\tau_j)|\dot\Theta_j|/(4\pi c_0^2\Omega R)$. Dropping the absolute value and the root sum requires the subsonic assumption. At $1-M_r=0$ the ideal point-source expression has a [caustic](../../../../../../wave-caustic.md); finite source size and bandwidth regularize that idealization.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
