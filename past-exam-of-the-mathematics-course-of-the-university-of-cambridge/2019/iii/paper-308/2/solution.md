<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Away from a zero of $\phi$, the first [Bogomolny vortex equation](../../../../../bogomolny-vortex-equation.md) gives

$$
a_{\bar z}=-i\partial_{\bar z}\log\phi,
\qquad
f_{z\bar z}=-2i\partial_z\partial_{\bar z}\log|\phi|.
$$

Substitution into the second equation, with $\nabla^2=4\partial_z\partial_{\bar z}$, gives

$$
\boxed{-\frac2\Omega\nabla^2\log|\phi|=1-|\phi|^2}.
$$

Now set $\widetilde\Omega=\Omega|\phi|^2$. The [Gaussian curvature](../../../../../gaussian-curvature.md) formula gives

$$
\widetilde K\widetilde\Omega=K\Omega-\nabla^2\log|\phi|.
$$

Therefore $(\widetilde K+1/2)\widetilde\Omega=(K+1/2)\Omega$ implies

$$
-\nabla^2\log|\phi|=\frac\Omega2(1-|\phi|^2),
$$

which is exactly the vortex equation.

The metric

$$
ds_n^2=\frac{8n^2|z|^{2n-2}}{(1-|z|^{2n})^2}dzd\bar z
$$

is the pullback of the $n=1$ [Poincare disc model](../../../../../poincare-disk-model.md) metric under $w=z^n$. It consequently has $K=-1/2$ away from the origin. Comparing it with $ds_1^2$ gives the [Witten hyperbolic vortex](../../../../../witten-hyperbolic-vortex.md)

$$
\boxed{|\phi|=\frac{n|z|^{n-1}(1-|z|^2)}{1-|z|^{2n}}}.
$$

Putting $n=N+1$ gives winding number $N$. A gauge choice with positive radial factor is

$$
\phi=\frac{n z^N(1-|z|^2)}{1-|z|^{2n}},
$$

and then

$$
\boxed{
a_{\bar z}=i\left(\frac{z}{1-|z|^2}-\frac{nz|z|^{2n-2}}{1-|z|^{2n}}\right),
\qquad a_z=\overline{a_{\bar z}}.
}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
