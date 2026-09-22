<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

[Kelvin's circulation theorem](../../../../../kelvin-s-circulation-theorem.md) states that a smooth inviscid barotropic fluid subject to a conservative body force preserves [circulation](../../../../../circulation-physics.md) around every closed [material curve](../../../../../material-curve.md). Write the [pressure](../../../../../pressure.md) term as $\nabla w$ with $dw=dp/\rho$, and the body force per mass as $-\nabla\Phi$. Then the [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) give $D\mathbf u/Dt=-\nabla(w+\Phi)$. For a moving parametrization $\mathbf x(s,t)$ with $\partial_t\mathbf x=\mathbf u$,

$$
\begin{aligned}
\frac d{dt}\oint_{C(t)}\mathbf u\cdot d\mathbf x
&=\oint_{C(t)}\frac{D\mathbf u}{Dt}\cdot d\mathbf x
+\oint_{C(t)}\mathbf u\cdot d\mathbf u\\
&=\oint_{C(t)}\nabla\left(\frac12u^2-w-\Phi\right)\cdot d\mathbf x=0.
\end{aligned}
$$

The last integral is the increment of a single-valued scalar around a closed curve. Consequently

$$
\boxed{\Gamma(C(t))=\Gamma(C(0))}.
$$

Constant density is a special barotropic case with $w=p/\rho$. Viscosity, nonconservative forcing or baroclinic [pressure](../../../../../pressure.md) gradients can invalidate this conservation law; the exterior-cylinder conclusions use the smooth inviscid hypotheses.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
