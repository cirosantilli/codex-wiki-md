<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an inviscid [Boussinesq approximation](../../../../../../boussinesq-approximation.md) fluid in a nonrotating frame, write buoyancy as $\sigma$ and kinematic pressure as $p$. The governing equations are

$$
\frac{D\mathbf u}{Dt}=-\nabla p+\sigma\widehat{\mathbf z},
\qquad
\frac{D\sigma}{Dt}=0,
\qquad
\nabla\mathbin\cdot\mathbf u=0.
$$

They require density variations to be small compared with a constant reference density, while retaining those variations in [buoyancy](../../../../../../buoyancy.md); the flow scale must be small compared with the background density scale height. Ideal flow additionally neglects viscosity and scalar diffusion.

Linearize about

$$
\overline{\mathbf u}=\overline u(z)\widehat{\mathbf x},
\qquad
\frac{d\overline\sigma}{dz}=N^2(z)>0,
$$

where $N$ is the [buoyancy frequency](../../../../../../buoyancy-frequency.md), and define

$$
D_t=\partial_t+\overline u\,\partial_x.
$$

For two-dimensional disturbances, the linear equations are

$$
\boxed{D_tu'+\overline u_z w'=-p'_x},
$$



$$
\boxed{D_tw'=-p'_z+\sigma'},
$$



$$
\boxed{D_t\sigma'+N^2w'=0},
$$



$$
\boxed{u'_x+w'_z=0}.
$$

The condition $N^2>0$ expresses [stable density stratification](../../../../../../stable-density-stratification.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
