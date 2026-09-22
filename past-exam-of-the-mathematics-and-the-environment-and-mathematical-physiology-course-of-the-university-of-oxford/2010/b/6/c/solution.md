<h1 id="b/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the period-one inner product $\langle Y,V\rangle=\int_0^1Y(\sigma)\cdot V(\sigma)\,d\sigma$. Periodic [integration by parts](../../../../../integration-by-parts.md) gives $\widehat L^*Y=-Y'-DF(U)^{\mathsf T}Y$. Let $Y$ span this adjoint [null space](../../../../../kernel-of-a-linear-map-split.md) and normalize $\int_0^1Y\cdot U'\,d\sigma=1$. For oscillator $i$, write $s=\sigma+\theta_i(\tau)$. Then $\partial_\tau u_{i,0}=\theta_i'U'(s)$ and $\partial_\sigma u_{i,0}=U'(s)$.

The [Fredholm solvability condition](../../../../../fredholm-solvability-condition.md) makes the forcing in the order-$\epsilon$ equation orthogonal to $Y(s)$. Its intrinsic and [frequency](../../../../../frequency.md) terms integrate to $\xi_i-\Omega_1-\theta_i'$, where

$$
\boxed{\xi_i=\int_0^1\sum_{a=1}^mY^a(s)G_i^a(U(s))\,ds.}
$$

Voltage-only coupling contributes

$$
\sum_jd_{ij}\int_0^1Y^1(s)[U^1(s+\theta_j-\theta_i)-U^1(s)]\,ds.
$$

Thus with

$$
\boxed{h(\phi)=\int_0^1Y^1(s)U^1(s+\phi)\,ds}
$$

the complete phase equation is

$$
\boxed{\theta_i'=\xi_i-\Omega_1+\sum_jd_{ij}[h(\theta_j-\theta_i)-h(0)].}
$$

Periodicity makes these formulae independent of the absolute initial phase. The adjoint [function](../../../../../function-split.md) is a [phase response function](../../../../../phase-response-function.md); it projects a small perturbation of each state component onto its accumulated phase change. The subtraction of $h(0)$ ensures zero coupling between identical phases, as required by the original [voltage](../../../../../voltage.md) differences. The source's reference to its equation (1) is read as the uncoupled cycle equation, numbered (3) on the actual page.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
