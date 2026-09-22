<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

Substitution of the separated exponential profile into the [age-structured population equation](../../../../../age-structured-population-equation.md) gives $r'=-(\gamma+\mu(a))r$. Therefore

$$
r(a)=C\exp\!\left[-\gamma a-\int_0^a\mu(s)\,ds\right].
$$

For $C\ne0$, the birth boundary condition cancels $C$ and becomes the [Euler-Lotka equation](../../../../../euler-lotka-equation.md)

$$
\boxed{\int_0^\infty b(a)\exp\!\left[-\gamma a-\int_0^a\mu(s)\,ds\right]da=1}.
$$

The survival probability to age $a$ is $e^{-\mu a}$ for constant death rate. Hence the expected lifetime offspring count, or [net reproduction rate](../../../../../net-reproduction-rate.md), is

$$
\boxed{R_0=\int_0^\infty Ba^pe^{-(\lambda+\mu)a}\,da
=\frac{Bp!}{(\lambda+\mu)^{p+1}}}.
$$

The [Gamma integral](../../../../../gamma-integral.md) evaluates the [Euler-Lotka equation](../../../../../euler-lotka-equation.md) as $Bp!/(\lambda+\mu+\gamma)^{p+1}=1$, requiring $\lambda+\mu+\gamma>0$. Its real solution and profile are

$$
\boxed{\gamma=(Bp!)^{1/(p+1)}-\lambda-\mu,\qquad
n(a,t)=C e^{\gamma t}e^{-[(Bp!)^{1/(p+1)}-\lambda]a}}.
$$

Thus **$B^*=(\lambda+\mu)^{p+1}/p!$**, and $B>B^*$ gives positive growth. The profile is a nonzero formal separated solution for all positive $B$; a finite total population additionally requires $\gamma+\mu>0$, equivalently $(Bp!)^{1/(p+1)}>\lambda$. A decaying-in-time mode need not have an integrable age profile.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
