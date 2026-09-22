<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

The [derivative](../../../derivative.md) formula requires additional regularity: continuity alone does not define $f'$. Assume $f$ is continuously differentiable, or locally absolutely continuous with its almost-everywhere [derivative](../../../derivative.md). Integration by parts on $[0,R]$ gives

$$
\int_0^Re^{-pt}f'(t)dt=e^{-pR}f(R)-f(0)+p\int_0^Re^{-pt}f(t)dt.
$$

For $\operatorname{Re}p>c$, the given exponential bound makes the first term tend to zero. Thus the improper transform exists under these regularity assumptions and

$$
\boxed{\widehat{f'}(p)=p\widehat f(p)-f(0).}
$$

For the primitive, absolute integrability justifies reversing the integration order:

$$
\widehat h(p)=\int_0^\infty f(s)\int_s^\infty e^{-pt}dt\,ds
=\boxed{\frac{\widehat f(p)}p}.
$$

Indeed the corresponding absolute double integral is finite when $\operatorname{Re}p>c$.

For real $p>0$, substitution $t=s^2/p$ and the supplied [Gaussian integral](../../../gaussian-integral.md) give

$$
\mathcal L[t^{-1/2}](p)=\frac2{\sqrt p}\int_0^\infty e^{-s^2}ds
=\boxed{\sqrt\pi\,p^{-1/2}.}
$$

Both sides are [holomorphic](../../../holomorphic-function-split.md) for $\operatorname{Re}p>0$, so the [identity theorem](../../../identity-theorem.md) extends this equality there, taking the square root with positive real part. The integrable singularity at zero causes no difficulty for this improper integral. The primitive rule then gives $\mathcal L[2\sqrt t]=\sqrt\pi\,p^{-3/2}$.

For the conductor, take the [Laplace transform](../../../laplace-transform.md) in time and write $U(x,p)$. The initial temperature gives $U_{xx}=pU$. Use the usual physical condition that the temperature is bounded far down the conductor; this selects the decaying solution

$$
U(x,p)=A(p)e^{-\sqrt p\,x},\qquad\operatorname{Re}\sqrt p>0.
$$

The constant applied flux has transform $Q/p$, so $-kU_x(0,p)=Q/p$, giving $A(p)=Q/(kp^{3/2})$. This is the [surface temperature under constant heat flux on a half-line](../../../surface-temperature-under-constant-heat-flux-on-a-half-line.md). Using the transform just calculated yields

$$
\boxed{u(0,t)=\frac{2Q}{k\sqrt\pi}\sqrt t\qquad(t>0).}
$$

Here $k>0$ is the [thermal conductivity](../../../thermal-conductivity.md). The far-field boundedness is the customary physical selection condition; without a spatial growth restriction the written PDE and initial/boundary data alone do not specify that selection. Within the physical solution, the face temperature tends continuously to zero as $t\downarrow0$.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2004](../../2004-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
