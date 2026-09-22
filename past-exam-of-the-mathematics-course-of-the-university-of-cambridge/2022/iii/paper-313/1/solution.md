<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write the [scalar field](../../../../../scalar-field.md) energy as $E=T+V$, where

$$
T=\frac12\int_{-\infty}^{\infty}(\phi')^2\,dx,
\qquad
V=\int_{-\infty}^{\infty}U(\phi)\,dx.
$$

Under the [Derrick scaling](../../../../../derrick-scaling.md) $\phi_\lambda(x)=\phi(\lambda x)$, a [change of variables](../../../../../change-of-variables-formula.md) gives

$$
E(\lambda)=\lambda T+\lambda^{-1}V.
$$

A finite-energy solution of the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is stationary under this admissible variation. The [Derrick virial identity](../../../../../derrick-virial-identity.md) is therefore

$$
0=E'(1)=T-V,
\qquad
\boxed{\frac12\int_{-\infty}^{\infty}(\phi')^2\,dx
=\int_{-\infty}^{\infty}U(\phi)\,dx}.
$$

The static field equation is $\phi''=U'(\phi)$, so integration gives

$$
U(\phi)=\frac12\phi^6-\phi^4+\frac12\phi^2+C
=\frac12\phi^2(1-\phi^2)^2+C.
$$

The polynomial before $C$ is nonnegative and vanishes, so requiring the minimum to be zero fixes $C=0$. Hence the [vacuum manifold](../../../../../vacuum-manifold.md) is

$$
\boxed{U^{-1}(0)=\{-1,0,1\}},
$$

which has three elements. A finite-energy [scalar-field kink](../../../../../scalar-field-kink.md) can join only adjacent vacua: a solution cannot cross the intermediate vacuum at finite $x$ because its first integral would have $\phi=\phi'=0$ there and the [Picard-Lindelöf theorem](../../../../../picard-lindelof-theorem.md) would make it constant. There are therefore four oriented topological sectors,

$$
-1\to0,\qquad0\to-1,\qquad0\to1,\qquad1\to0,
$$

comprising two increasing kinks and their two antikinks. Symmetry under $\phi\mapsto-\phi$ and spatial reflection generates all four from one profile.

For the $0\to1$ sector, completing the square gives the [Bogomolny bound](../../../../../bogomolny-bound.md)

$$
\begin{aligned}
E
&=\frac12\int_{-\infty}^{\infty}
\left[\phi'-\phi(1-\phi^2)\right]^2dx
+\int_{-\infty}^{\infty}\phi'\phi(1-\phi^2)\,dx\\
&\geq\int_0^1\phi(1-\phi^2)\,d\phi.
\end{aligned}
$$

Equality holds for the [Bogomolny equation](../../../../../bogomolny-equations.md)

$$
\boxed{\phi'=\phi(1-\phi^2)}.
$$

With $y=\phi^2$, this becomes the [logistic differential equation](../../../../../logistic-differential-equation.md) $y'=2y(1-y)$. Translation invariance supplies an arbitrary center $x_0$, and the explicit [kink in a phi-six model](../../../../../kink-in-a-phi-six-model.md) is

$$
\boxed{\phi(x)=\frac1{\sqrt{1+e^{-2(x-x_0)}}}}.
$$

It tends to $0$ and $1$ at the two spatial ends and saturates the bound. Its mass is consequently

$$
\boxed{M=\int_0^1\phi(1-\phi^2)\,d\phi=\frac14}.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 313](../../paper-313-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
