<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret derivatives on the space of symmetric [strains](../../../../../../strain.md), with inner product $A:B=A_{ij}B_{ij}$. Assume a differentiable [strain energy density](../../../../../../strain-energy-density.md) with local [stress](../../../../../../stress.md) $\sigma=D_\varepsilon W$, and a differentiable stable equilibrium branch under the prescribed affine boundary [displacement](../../../../../../displacement.md). Thus $u_E(x)=Ex+v_E(x)$ with $v_E=0$ on $\partial\Omega$; part(a) ensures that the mean [strain](../../../../../../strain.md) is exactly $E$.

Vary $E$ in any symmetric direction $H$. The induced displacement variation has the form $\dot u=Hx+\dot v$, where $\dot v$ vanishes on the boundary. Differentiating the [effective elastic energy](../../../../../../effective-elastic-energy.md) and using [static elastic equilibrium](../../../../../../static-elastic-equilibrium.md) gives

$$
\begin{aligned}
DW^{\mathrm{eff}}(E):H
&=\frac1{|\Omega|}\int_\Omega\sigma:\operatorname{sym}\nabla\dot u\,dx\\
&=\langle\sigma\rangle:H+
\frac1{|\Omega|}\int_\Omega\sigma:\operatorname{sym}\nabla\dot v\,dx\\
&=\langle\sigma\rangle:H.
\end{aligned}
$$

The last term is zero by [integration by parts](../../../../../../integration-by-parts.md), since the [body force](../../../../../../body-force.md) is zero and $\dot v$ has zero boundary trace. As $H$ is arbitrary,

$$
\boxed{DW^{\mathrm{eff}}(E)=\langle\sigma\rangle.}
$$

This is a work-conjugacy statement on symmetric [tensors](../../../../../../tensor.md); treating off-diagonal entries as independent scalar coordinates without their contraction weights would introduce erroneous factors of two. If the minimized [effective elastic energy](../../../../../../effective-elastic-energy.md) has a nondifferentiable point, the corresponding formulation uses a [subgradient](../../../../../../subgradient.md) rather than a claimed classical derivative.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
