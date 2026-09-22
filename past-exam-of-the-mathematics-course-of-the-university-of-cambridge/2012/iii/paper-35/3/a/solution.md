<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D$ be the unit disc and normalize its positive [Poisson kernel](../../../../../../poisson-kernel-for-the-upper-half-plane.md) at the boundary point $1$ by

$$
h(z)=\frac{1-|z|^2}{|1-z|^2},\qquad h(0)=1.
$$

It is harmonic in $D$. Let $p_D(t,z,w)$ be the killed [Brownian transition density](../../../../../../brownian-transition-density.md), for [planar Brownian motion](../../../../../../planar-brownian-motion.md) with generator $\tfrac12\Delta$. The [Doob h-transform](../../../../../../doob-h-transform.md) has sub-Markov transition density

$$
\boxed{p_D^h(t,z,w)=p_D(t,z,w)\frac{h(w)}{h(z)}.}
$$

Its missing mass represents paths already absorbed at the distinguished boundary point. Equivalently, for a stopping time $\sigma$ before exit from a compact subdomain, its law is weighted relative to ordinary killed [Brownian motion](../../../../../../brownian-motion-split.md) by $h(B_\sigma)/h(B_0)$. These stopped laws are consistent and define a diffusion up to its lifetime. Its generator is

$$
\mathcal L^hf=\frac1h\frac12\Delta(hf)=\frac12\Delta f+\nabla\log h\cdot\nabla f.
$$

This is a rigorous [Brownian motion conditioned to exit at a boundary point](../../../../../../brownian-motion-conditioned-to-exit-at-a-boundary-point.md), not conditioning on an event of positive probability. Exhaustion of $D$ shows that its terminal boundary limit is $1$; its lifetime is finite. For example its expected lifetime from $0$ is $\int_DG_D^{\mathrm{BM}}(0,w)h(w)\,dw$, which is finite: the Green function vanishes linearly near the smooth boundary and cancels the Poisson-kernel singularity there, while its logarithmic singularity at $0$ is integrable.

One can also condition ordinary [Brownian motion](../../../../../../brownian-motion-split.md) on exiting through an arc $I_\epsilon$ about $1$, and then let its length decrease to zero. The conditional harmonic functions $\omega_D(z,I_\epsilon)/\omega_D(0,I_\epsilon)$ converge locally uniformly to $h(z)$. Thus their stopped conditional laws converge to this same diffusion. Both constructions specify the conditioning unambiguously.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
