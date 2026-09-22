<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Here is a direct use of the spherical representation that also avoids estimating separate coordinate [derivatives](../../../../../../derivative.md) at the poles. Put $A=\Delta_{S^2}$, $T=\partial_r^2+2r^{-1}\partial_r$, and write $d\omega$ for unit-sphere area. Then $f=Tu+r^{-2}Au$. Expanding its squared [norm](../../../../../../norm.md) with the physical measure gives

$$
\|f\|_2^2=\|Tu\|_2^2+\|r^{-2}Au\|_2^2+2\int_{1/2}^2\!\int_{S^2}(Tu)(Au)\,d\omega\,dr.
$$

On each boundary sphere $u=0$, so every angular [derivative](../../../../../../derivative.md), including $Au$ and $\nabla_Su$, is zero there. Radial and angular [integration by parts](../../../../../../integration-by-parts.md) consequently give

$$
\int(Tu)(Au)=\int|\nabla_Su_r|^2-\int r^{-2}|\nabla_Su|^2.
$$

Indeed the $u_{rr}$ term gives $\int|\nabla_Su_r|^2$ with boundary remainder $[\int u_rAu]=0$, while the $2u_r/r$ term is $-\int r^{-1}\partial_r|\nabla_Su|^2=-\int r^{-2}|\nabla_Su|^2$, its boundary remainder also being zero. Thus

$$
\|Tu\|_2^2+\|r^{-2}Au\|_2^2+2\int|\nabla_Su_r|^2
=\|f\|_2^2+2\int r^{-2}|\nabla_Su|^2\le C\|f\|_2^2,
$$

where the last step uses the preceding $H^1$ energy estimate and $r\ge1/2$. All unmarked integrals in these two identities are with $dr\,d\omega$.

To control every angular second [derivative](../../../../../../derivative.md), the [spherical Hessian identity](../../../../../../spherical-hessian-identity.md) is

$$
\int_{S^2}|\nabla_S^2w|^2=\int_{S^2}(Aw)^2-\int_{S^2}|\nabla_Sw|^2.
$$

It follows by integrating the derivative-commutation identity $\nabla^a\nabla_a\nabla_bw=\nabla_bAw+\operatorname{Ric}_b{}^c\nabla_cw$ and using $\operatorname{Ric}=h$ on the unit sphere. There is no sphere boundary. Hence the preceding bound controls $\nabla_S^2u$, $\nabla_Su_r$, and $u_{rr}=Tu-2u_r/r$ in their appropriate weighted [norms](../../../../../../norm.md).

In an orthonormal polar frame the Cartesian [Hessian matrix](../../../../../../hessian-matrix.md) has components

$$
D^2u(e_r,e_r)=u_{rr},\quad D^2u(e_r,e_A)=r^{-1}(\nabla_Su_r)_A-r^{-2}(\nabla_Su)_A,
$$

and $D^2u(e_A,e_B)=r^{-2}(\nabla_S^2u)_{AB}+r^{-1}u_r\delta_{AB}$. Since $r$ is bounded above and below, these bounds plus the first-order estimate prove

$$
\boxed{\|u\|_{H^2(\Omega)}\le C\|f\|_2.}
$$

This is the [direct spherical-shell H2 estimate](../../../../../../direct-spherical-shell-h2-estimate.md). Intrinsic angular integration combines the suggested angular tests, with no spurious boundary at the polar coordinate singularities.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
