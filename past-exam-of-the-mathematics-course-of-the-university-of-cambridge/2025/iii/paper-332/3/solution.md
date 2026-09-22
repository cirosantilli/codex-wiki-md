<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [shelfy stream](../../../../../shelfy-stream.md) is grounded ice with nearly depth-independent horizontal velocity. If the lubricating till has thickness $d$ and viscosity $\mu_t$, its simple-shear traction is approximately $\mu_tu/d$. Comparison with $\tau_b=\mu u/\lambda$ gives

$$
\boxed{\lambda\sim\frac{\mu}{\mu_t}d,}
$$

so $\lambda$ has dimensions of length.

Hydrostatic pressure contributes the depth-integrated longitudinal force $-\rho gh^2/2$, while the Newtonian extensional stress contributes $4\mu h u_x$ by the [shallow-shelf approximation](../../../../../shallow-shelf-approximation.md). Balancing the change of their sum against basal drag on a slice gives

$$
\boxed{4\mu(hu_x)_x-\rho ghh_x-\mu\frac u\lambda=0.}
$$

For a freely floating [ice shelf](../../../../../ice-shelf.md), hydrostatic flotation reduces the gravitational driving by $1-\rho/\rho_w$ and removes basal drag:

$$
\boxed{4\mu(hu_x)_x-
ho g\left(1-\frac\rho{\rho_w}\right)hh_x=0.}
$$

Depth-integrated [mass conservation](../../../../../mass-conservation.md) is

$$
\boxed{h_t+(hu)_x=0}
$$

in the absence of accumulation or ablation.

In a thin stream with horizontal scale $L_x$, the ratio of extensional resistance to basal drag is $O(\lambda h/L_x^2)$, which is small when the thin-film condition $h/L_x\ll1$ is combined with $\lambda\ll h_G$. For steady flux $hu=q$, neglecting extension gives

$$
\rho ghh_x=-\frac{\mu q}{\lambda h}.
$$

At the [grounding line](../../../../../grounding-line.md), flotation over a bed depth $b$ gives

$$
\boxed{h_G=\frac{\rho_w}{\rho}b.}
$$

Integration yields

$$
\boxed{
h=h_G\left(1-\frac x\delta\right)^{1/3},
\qquad
\delta=\frac{\rho g\lambda h_G^3}{3\mu q},
\qquad \alpha=\frac13.}
$$

The grounding-line slope is $|h_x(0)|=\mu q/(\rho g\lambda h_G^2)$. Thin-film theory therefore also requires

$$
\boxed{\lambda\gg\frac{\mu q}{\rho g h_G^2}.}
$$

This and $\lambda\ll h_G$ are compatible precisely when $\mu q/(\rho gh_G^3)\ll1$.

The total horizontal force resultant in the stream is

$$
N=4\mu h u_x-\frac12\rho gh^2.
$$

The floating shelf equations and its ocean-front traction imply that the force it exerts at the grounding line is the ocean's hydrostatic force, so

$$
N(0)=-\frac12\rho_wgb^2.
$$

Using flotation and the approximate stream solution,

$$
u_x(0)=-\frac q{h_G^2}h_x(0)
=\frac{\mu q^2}{\rho g\lambda h_G^4}.
$$

Consequently

$$
4\mu h_Gu_x(0)
=\frac12\rho gh_G^2\left(1-\frac\rho{\rho_w}\right),
$$

and the grounding-line flux-thickness relation is

$$
\boxed{
q=\frac{\rho g}{2\sqrt2\,\mu}
\left[\lambda h_G^5\left(1-\frac\rho{\rho_w}\right)\right]^{1/2}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
