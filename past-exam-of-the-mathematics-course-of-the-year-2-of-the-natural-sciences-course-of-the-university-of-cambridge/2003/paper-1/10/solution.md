<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Choose homogeneous [Dirichlet boundary conditions](../../../../dirichlet-boundary-condition.md), $y(a)=y(b)=0$, and nonzero admissible [functions](../../../../function-split.md) with finite $F$ and positive $G$. Variations obey the same zero endpoint values. At a stationary [Rayleigh quotient](../../../../rayleigh-quotient.md), set $\lambda=F[y]/G[y]$. Then

$$
0=G\,\delta\Lambda=\delta F-\lambda\delta G=2[py'\eta]_a^b+2\int_a^b\left[-(py')'+qy-\lambda wy\right]\eta\,dx.
$$

The boundary term vanishes, and the [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) gives the [Sturm-Liouville equation](../../../../sturm-liouville-equation.md) $-(py')'+qy=\lambda wy$. Thus stationary [functions](../../../../function-split.md) are [eigenfunctions](../../../../eigenfunction.md). Conversely, multiply that equation by $y$ and integrate by parts to obtain $F=\lambda G$; its first [variation](../../../../variation.md) then vanishes by the same calculation. This proves that stationary values are the corresponding [eigenvalues](../../../../eigenvalue.md). Homogeneous [Neumann boundary conditions](../../../../neumann-boundary-condition.md) also make the displayed boundary terms vanish; general [Robin boundary conditions](../../../../robin-boundary-condition.md) can require a boundary contribution to the quadratic form.

For $p=1$, $q=0$, $w=x$ on $(0,\pi)$, the [polynomial](../../../../polynomial-split.md) [trial function](../../../../trial-function.md) $y=x(\pi-x)$ satisfies the endpoint conditions. Its [Rayleigh quotient](../../../../rayleigh-quotient.md) uses

$$
F=\int_0^\pi(\pi-2x)^2dx=\frac{\pi^3}3,\qquad G=\int_0^\pi x^3(\pi-x)^2dx=\frac{\pi^6}{60},
$$

so the [polynomial](../../../../polynomial-split.md) estimate is $\boxed{\lambda_{\rm poly}=20/\pi^3\simeq0.64503}$. The trigonometric [trial function](../../../../trial-function.md) $y=\sin x$ gives

$$
F=\frac\pi2,\qquad G=\int_0^\pi x\sin^2x\,dx=\frac{\pi^2}4,
$$

and hence $\boxed{\lambda_{\rm trig}=2/\pi\simeq0.63662}$. Both are **upper bounds** on the lowest [eigenvalue](../../../../eigenvalue.md), by the [Rayleigh-Ritz method](../../../../rayleigh-ritz-method.md); neither trial is an exact [eigenfunction](../../../../eigenfunction.md), so the inequalities are strict.

Their closeness has a useful explanation beyond their similar single-arch shapes. Both [trial functions](../../../../trial-function.md) are symmetric under $x\mapsto\pi-x$, forcing $\int_0^\pi xy^2dx=(\pi/2)\int_0^\pi y^2dx$. The [reflection-symmetric trials for a linearly weighted Rayleigh quotient](../../../../reflection-symmetric-trials-for-a-linearly-weighted-rayleigh-quotient.md) therefore reduce this problem to a constant multiple of the ordinary Dirichlet energy quotient. The [sine](../../../../sine.md) is the best trial within this symmetric class, and the [polynomial](../../../../polynomial-split.md)'s value is only a factor $10/\pi^2\simeq1.0132$ larger. The unrestricted lowest [eigenfunction](../../../../eigenfunction.md) can be asymmetric because the weight $x$ is asymmetric.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 1](../../paper-1-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
