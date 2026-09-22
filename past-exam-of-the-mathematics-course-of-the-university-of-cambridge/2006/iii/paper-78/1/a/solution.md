<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $n$ point out of the drop, and use $-$ for the interior and $+$ for the exterior. The interfacial [velocity](../../../../../../velocity.md) is continuous. Define $\kappa=\nabla_s\cdot n$; for a sphere of radius $a$ it is $2/a$. With constant [surface tension](../../../../../../surface-tension.md), the [interfacial stress balance with variable surface tension](../../../../../../interfacial-stress-balance-with-variable-surface-tension.md) reduces to

$$
(\sigma^+-\sigma^-)n=\gamma\kappa n.
$$

Use the exterior-viscosity kernels to define $S[t]=\int J(y-x)t(x)\,dS_x$ and $D[u]=\int u(x)K(y-x)n(x)\,dS_x$. The interior [viscosity](../../../../../../dynamic-viscosity.md) is $\lambda\mu$, so its [velocity](../../../../../../velocity.md) kernel is $J/\lambda$, while its [stress](../../../../../../stress.md) kernel $K$ is unchanged. The interior boundary equation is

$$
\frac\lambda2u=S[\sigma^-n]+\lambda D[u].
$$

For the decaying exterior flow, the inner boundary's fluid-domain normal is $-n$, so

$$
\frac12u=-S[\sigma^+n]-D[u].
$$

Add these equations and use the [traction](../../../../../../traction.md) jump. The required [capillary boundary integral equation for a viscous drop](../../../../../../capillary-boundary-integral-equation-for-a-viscous-drop.md) is

$$
\boxed{\frac{1+\lambda}{2}u(y)
=-\gamma\int_{\partial V}J(y-x)\kappa(x)n(x)\,dS_x
+(\lambda-1)\int_{\partial V}u(x)K(y-x)n(x)\,dS_x.}
$$

The formula uses the drop-outward normal consistently in both integrals. If $\lambda=1$, the double-layer term cancels. A spherical drop of constant curvature has zero [velocity](../../../../../../velocity.md): a constant Laplace-pressure jump is balanced without motion. A prescribed ambient flow would add its known far-boundary contribution; none is present for the surface-tension-driven flow here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
