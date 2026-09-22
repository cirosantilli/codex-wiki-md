<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Interpret $L=-\Box$ as the minimally coupled scalar [positive Laplace-Beltrami operator](../../../../../positive-laplace-beltrami-operator.md) on the smooth [closed manifold](../../../../../closed-manifold.md). Writing $dV$ for its metric volume measure (the [Riemannian volume form](../../../../../riemannian-volume-form.md) on an oriented chart), integration by parts gives $\langle u,Lu\rangle=\int_M|\nabla u|^2dV\ge0$. The [compact elliptic spectral theorem](../../../../../compact-elliptic-spectral-theorem.md) supplies an orthonormal basis $u_j$ with $Lu_j=\lambda_j u_j$, real nonnegative [eigenvalues](../../../../../eigenvalue.md) tending to infinity and finite multiplicities. Solve this eigenvalue problem to obtain the [spectral zeta function](../../../../../spectral-zeta-function.md)

$$
\boxed{\zeta_L(s)=\sum_{\lambda_j>0}\lambda_j^{-s},\qquad \operatorname{Re}s>d/2.}
$$

The zero [eigenvalues](../../../../../eigenvalue.md) are excluded, not assigned inverse powers. Their multiplicity $n_0$ is the number of connected components: $Lu=0$ implies $\int|\nabla u|^2dV=0$, so $u$ is constant on each component.

An equivalent calculation uses the [spectral expansion of the Riemannian heat kernel](../../../../../spectral-expansion-of-the-riemannian-heat-kernel.md),

$$
K(t;x,y)=\sum_j e^{-t\lambda_j}u_j(x)\overline{u_j(y)},\qquad
K(t)=\int_M K(t;x,x)dV=\sum_j e^{-t\lambda_j}.
$$

Since $\int_0^\infty t^{s-1}e^{-t\lambda}\,dt=\Gamma(s)\lambda^{-s}$ for $\lambda>0$, the [Mellin transform](../../../../../mellin-transform.md) gives

$$
\boxed{\zeta_L(s)=\frac1{\Gamma(s)}\int_0^\infty t^{s-1}(K(t)-n_0)\,dt.}
$$

The reduced trace decays exponentially at large $t$. At small $t$, subtract a finite number of terms of the [heat kernel expansion](../../../../../heat-kernel-expansion.md), integrate those terms explicitly, and then integrate the remainder. Increasing the number of subtractions extends the formula successively to further left half-planes, producing the [meromorphic continuation](../../../../../meromorphic-continuation.md) of $\zeta_L$ rather than substituting $s=0$ in its divergent defining series.

For completeness, the needed curvature coefficient comes from the [heat-kernel transport equations](../../../../../heat-kernel-transport-equations.md). In [normal coordinates](../../../../../normal-coordinates.md) $\xi$ centered at $y$, the [Riemannian volume form](../../../../../riemannian-volume-form.md) has density $J(\xi)=1-\tfrac16R_{ab}(y)\xi^a\xi^b+O(|\xi|^3)$. The leading Gaussian amplitude is therefore

$$
u_0(x,y)=J(\xi)^{-1/2}=1+\frac1{12}R_{ab}(y)\xi^a\xi^b+O(|\xi|^3).
$$

Substitution of the Gaussian amplitude series into the heat equation gives the first diagonal transport relation $u_1(y,y)=\Box_xu_0(x,y)|_{x=y}=R(y)/6$. The [curvature coefficient of the scalar heat kernel](../../../../../curvature-coefficient-of-the-scalar-heat-kernel.md) is consequently

$$
K(t;x,x)\sim\frac1{(4\pi t)^{d/2}}\left(1+\frac t6R(x)+O(t^2)\right).
$$

In dimension two this implies

$$
K(t)=\frac{\operatorname{Area}(M)}{4\pi t}+\frac1{24\pi}\int_M R\,dV+O(t).
$$

Set $A_0=\operatorname{Area}(M)/(4\pi)$ and $A_1=\int_M R\,dV/(24\pi)$. Splitting the Mellin integral at $t=1$ and subtracting these two heat terms gives, near $s=0$,

$$
\zeta_L(s)=\frac1{\Gamma(s)}\left[\frac{A_0}{s-1}+\frac{A_1-n_0}{s}+H(s)\right],
$$

where $H$ is holomorphic for $\operatorname{Re}s>-1$. As $1/\Gamma(s)=s+O(s^2)$, only the second term survives at zero. Thus the [zero-mode correction to the spectral zeta value](../../../../../zero-mode-correction-to-the-spectral-zeta-value.md) is

$$
\boxed{\zeta_L(0)=\frac1{24\pi}\int_M R\,dV-n_0.}
$$

The [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md), with $R$ twice the Gaussian curvature, makes this $\boxed{\zeta_L(0)=\chi(M)/6-n_0}$. For a connected surface $n_0=1$, so the answer is $\chi(M)/6-1$; a sphere gives $-2/3$, and a flat torus gives $-1$.

The purely local heat coefficient is $A_1=\int R\,dV/(24\pi)$. Sometimes a formal formula for $\zeta(0)$ quotes this coefficient with zero modes left implicit. For the actual positive-spectrum [spectral zeta function](../../../../../spectral-zeta-function.md) defined above, the compact scalar problem necessarily has the additional subtraction $-n_0$. A strictly positive shifted operator is a different problem and has its own heat coefficients.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
