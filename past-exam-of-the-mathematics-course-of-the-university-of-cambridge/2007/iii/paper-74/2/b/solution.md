<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [normalized stationary fluctuation-dissipation relation for a reaction network](../../../../../../normalized-stationary-fluctuation-dissipation-relation-for-a-reaction-network.md) is

$$
\boxed{M\eta+\eta M^{\mathsf T}=D,\qquad
\eta_{ij}=\frac{\operatorname{Cov}(X_i,X_j)}{\mu_i\mu_j}.}
$$

Here $M$ is the negative drift [Jacobian matrix](../../../../../../jacobian-matrix.md) expressed in normalized population coordinates, and $D$ is the normalized noise matrix. More explicitly, with $S=\operatorname{diag}(\mu_i)$, drift Jacobian $A$, [stoichiometric vectors](../../../../../../stoichiometric-vector.md) $\nu_r$, and stationary [reaction propensity functions](../../../../../../reaction-propensity-function.md) $a_r$, these matrices are $M=-S^{-1}AS$ and $D=S^{-1}BS^{-1}$, where $B=\sum_ra_r\nu_r\nu_r^{\mathsf T}$. The [linear noise approximation](../../../../../../linear-noise-approximation.md) gives a covariance evolution $\dot\eta=-M\eta-\eta M^{\mathsf T}+D$; stationarity is the displayed [Continuous Lyapunov equation](../../../../../../continuous-lyapunov-equation.md).

In one dimension, the normalized restoring coefficient is $M=H/\tau=1/(2\tau)$. Squared chemical jumps determine the noise:

$$
B=9\lambda+\beta\sqrt\mu=12\lambda=\frac{4\mu}{\tau},\qquad
D=\frac{B}{\mu^2}=\frac4{\tau\mu}.
$$

The factor nine from a birth burst is essential; its three molecules arise in one correlated reaction event. The scalar [Continuous Lyapunov equation](../../../../../../continuous-lyapunov-equation.md) is $2M\eta=D$, giving

$$
\boxed{\eta\approx\frac4\mu,\qquad \operatorname{Var}(X)\approx4\mu.}
$$

Equivalently, the normalized variance is $\langle s\rangle/(H\mu)=2/((1/2)\mu)$. The [Fano factor](../../../../../../fano-factor.md) is approximately four. This calculation uses the prescribed mean closure and the [linear noise approximation](../../../../../../linear-noise-approximation.md), so its small-relative-fluctuation regime is $\mu\gg1$; it is not an exact assertion for arbitrarily small molecular copy numbers.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
