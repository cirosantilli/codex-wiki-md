<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

Use [suffix notation](../../../../../einstein-notation.md), with repeated indices summed. Contracting the two [Levi-Civita symbols](../../../../../levi-civita-symbol.md) gives

$$
[\mathbf u\times(\nabla\times\mathbf A)]_i
=\epsilon_{ijk}u_j\epsilon_{klm}\partial_lA_m
=u_j(\partial_iA_j-\partial_jA_i).
$$

Applying the [product rule](../../../../../product-rule.md) to $h=A_iB_i$ and substituting the two evolution equations yields

$$
\begin{aligned}
\partial_t h
&=B_iu_j\partial_iA_j-B_iu_j\partial_jA_i+B_i\partial_i\psi
+A_iB_j\partial_ju_i-A_iu_j\partial_jB_i\\
&=B_i\partial_i(u_jA_j+\psi)-u_j\partial_j(A_iB_i).
\end{aligned}
$$

In the second line we renamed dummy indices in $A_iB_j\partial_ju_i$ and then combined product derivatives. Hence

$$
\boxed{f=\mathbf u\cdot\mathbf A+\psi,\qquad
\partial_t h=\mathbf B\cdot\nabla f-\mathbf u\cdot\nabla h.}
$$

No zero-divergence assumption was used in this local identity.

When both fields are [solenoidal vector fields](../../../../../solenoidal-vector-field.md), the [product rule for divergence](../../../../../product-rule-for-divergence.md) rewrites this as a [conservation law](../../../../../conservation-law.md):

$$
\partial_t h=\nabla\cdot(f\mathbf B-h\mathbf u).
$$

Because the volume is fixed, differentiation under its integral and the [divergence theorem](../../../../../divergence-theorem.md) give

$$
\frac{dH}{dt}=\int_{\partial V}(f\mathbf B-h\mathbf u)\cdot\mathbf n\,dS=0
$$

under the two tangency conditions. Thus **the volume integral is conserved**. This is [helicity conservation by tangent boundary conditions](../../../../../helicity-conservation-by-tangent-boundary-conditions.md); when $\mathbf B=\nabla\times\mathbf A$, the density is the [magnetic helicity](../../../../../magnetic-helicity.md) density.

For the given axisymmetric field, the [curl in spherical coordinates](../../../../../curl-in-spherical-coordinates.md) gives

$$
\begin{aligned}
B_r&=\frac1{r\sin\theta}\partial_\theta(\sin\theta A_\phi)
=2(a^2-r^2)\cos\theta,\\
B_\theta&=-\frac1r\partial_r(rA_\phi)
=(4r^2-2a^2)\sin\theta,\\
B_\phi&=\frac1r\partial_r(rA_\theta)=3ar\sin\theta.
\end{aligned}
$$

There are no $\phi$ derivatives and $A_r=0$. Consequently

$$
\begin{aligned}
h&=A_\theta B_\theta+A_\phi B_\phi\\
&=ar^2(4r^2-2a^2)\sin^2\theta+3ar^2(a^2-r^2)\sin^2\theta\\
&=\boxed{ar^2(a^2+r^2)\sin^2\theta.}
\end{aligned}
$$

The [volume form](../../../../../volume-form.md) in [spherical polar coordinates](../../../../../spherical-coordinate-system.md) is $r^2\sin\theta\,dr\,d\theta\,d\phi$, so

$$
\begin{aligned}
H&=2\pi a\int_0^a r^4(a^2+r^2)\,dr\int_0^\pi\sin^3\theta\,d\theta\\
&=\frac{8\pi a}{3}\left(\frac{a^7}{5}+\frac{a^7}{7}\right)
=\boxed{\frac{32\pi a^8}{35}.}
\end{aligned}
$$

Here $B_r=0$ at $r=a$, as required for the magnetic-field tangency condition in the conservation argument; tangency of $\mathbf u$ is a separate hypothesis.

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
