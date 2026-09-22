<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $u=\lambda v$ and let $n$ now mean number per area. During [time](../../../../../../time-in-physics.md) $T$, the two strips of [impact parameters](../../../../../../impact-parameter.md) between $b$ and $b+db$, on opposite sides of the trajectory, have combined area $2uT\,db$. Thus

$$
\boxed{dn=2nuT\,db=2n\lambda vT\,db.}
$$

The same straight-line [impulse approximation](../../../../../../impulse-approximation.md) gives a kick $2Gm/(bu)$. Summing its squared size over these encounters gives

$$
D_v=\frac{\langle|\Delta\mathbf v|^2\rangle}{T}=\frac{8G^2m^2n}{u}\int_{b_{\min}}^{b_{\max}}\frac{db}{b^2}\simeq\frac{8G^2m^2n}{u b_{\min}},
$$

assuming $b_{\max}\gg b_{\min}$. The relevant change is now the small random [speed](../../../../../../speed.md) $u$, not the full circular [speed](../../../../../../speed.md) $v$. Setting $D_vt_{\rm rel}\sim u^2$ yields

$$
\boxed{t_{\rm rel}\simeq\frac{\lambda^3v^3b_{\min}}{8G^2m^2n}.}
$$

The [razor-thin disk relaxation](../../../../../../razor-thin-disk-relaxation.md) [integral](../../../../../../integral.md) is dominated by nearby encounters, rather than equally by logarithmic intervals. Because kicks cease to be weak near the cutoff, its numerical coefficient is an estimate.

Here the weak-deflection cutoff must use the relative [speed](../../../../../../speed.md): $b_{\min}\sim Gm/u^2=Gm/(\lambda^2v^2)$, which is larger than the spherical cutoff. Thus $t_{\rm rel}\sim u/(Gmn)$. Using $n\sim N/R^2$ and $v^2\sim GNm/R$ from the [virial theorem](../../../../../../virial-theorem.md) gives

$$
\boxed{t_{\rm rel}\sim\lambda\frac Rv=\lambda t_{\rm dyn}.}
$$

For example $n=N/(\pi R^2)$ gives the order-one coefficient $\pi/8$ in this last substitution; the paper's approximate equality suppresses such structural factors. The cancellation of $N$ is the central result.

An unsoftened point-particle system confined to an infinitesimally thin [plane](../../../../../../plane.md) is therefore **not collisionless over orbital times** for $\lambda\sim0.1$ in this encounter model. At fixed total [mass](../../../../../../mass.md), increasing $N$ decreases $m$ and the cutoff together; the enhanced importance of close planar encounters cancels the usual benefit of increasing particle number. This is a singular zero-thickness limit. A fixed nonzero [gravitational softening](../../../../../../gravitational-softening.md) length or physical thickness restores a different $N$ dependence, so the conclusion is not a prohibition on collisionless numerical models of disks.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
