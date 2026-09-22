<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Impermeability requires $\widehat w(-1)=\widehat w(1)=0$. Let $c=\omega/\alpha$ with real $\alpha\ne0$, and set $a=|\alpha|$. If $c$ is nonreal, or real outside the channel, the [Rayleigh equation for inviscid shear flow](../../../../../../../rayleigh-equation-for-inviscid-shear-flow.md) gives $\widehat w''-a^2\widehat w=0$ everywhere. The two wall conditions then force $\widehat w=0$. In fact there is no nonzero globally smooth eigenfunction for any $c$: the complete family is the [inviscid Couette continuous spectrum](../../../../../../../inviscid-couette-continuous-spectrum.md).

For each $\xi\in(-1,1)$, permit a localized [vorticity sheet](../../../../../../../vortex-sheet.md). Let $G_a$ be the [Dirichlet Green function](../../../../../../../dirichlet-green-function.md) satisfying $(D^2-a^2)G_a(z,\xi)=\delta(z-\xi)$. An explicit generalized [eigenfunction](../../../../../../../eigenfunction.md) is

$$
\boxed{\widehat w_\xi(z)=G_a(z,\xi)
=-\frac{\sinh[a(z_<+1)]\sinh[a(1-z_>)]}{a\sinh(2a)},\qquad
\omega_\xi=\alpha\xi,}
$$

where $z_<=\min(z,\xi)$ and $z_>=\max(z,\xi)$. It vanishes at both walls, is continuous at $z=\xi$, and has derivative jump $[\partial_zG_a]_{\xi^-}^{\xi^+}=1$. Consequently

$$
(z-\xi)(D^2-a^2)\widehat w_\xi=(z-\xi)\delta(z-\xi)=0,
$$

using the [Dirac delta multiplication identity](../../../../../../../dirac-delta-multiplication-identity.md). These are [vorticity-sheet eigenfunctions of inviscid Couette flow](../../../../../../../vorticity-sheet-eigenfunction-of-inviscid-couette-flow.md), understood as [generalized eigenfunctions](../../../../../../../generalized-eigenfunction.md), not as a discrete smooth [Sturm-Liouville eigenfunction expansion](../../../../../../../sturm-liouville-eigenfunction-expansion.md).

To see completeness, define the vorticity variable $q=(D^2-a^2)w$. Its evolution is $(\partial_t+i\alpha z)q=0$, so for any admissible initial vorticity $q_0$,

$$
\boxed{w(z,t)=\int_{-1}^1G_a(z,\xi)q_0(\xi)e^{-i\alpha\xi t}\,d\xi.}
$$

The homogeneous Dirichlet problem for $D^2-a^2$ has only the zero solution, so this inversion reconstructs every initial vertical-velocity field in its usual function space. The generalized frequencies fill the interval with endpoints $\pm\alpha$; the endpoint values are understood as the closure of the [continuous spectrum](../../../../../../../continuous-spectrum.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
