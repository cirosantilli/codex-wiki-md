<h1 id="22g/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Two function elements $(U,f)$ and $(V,g)$ define the same [germ of a holomorphic function](../../../../../../germ-of-a-holomorphic-function.md) at $p$ when $p\in U\cap V$ and they agree on some neighborhood of $p$. Write the germ as $[f]_p$. Basic open sets of the [space of germs of holomorphic functions](../../../../../../space-of-germs-of-holomorphic-functions.md) are

$$
\widetilde U_f=\{[f]_p:p\in U\},
$$

for open $U$ on which $f$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md). If two such sets meet, equality of the germs gives a smaller open sheet contained in their intersection, so these sets form a basis. The projection $\pi([f]_p)=p$ maps each sheet homeomorphically onto $U$. Compose this with a local coordinate on $X$ to define the complex charts on the germ space. Transition maps are the corresponding transition maps on $X$, hence [holomorphic](../../../../../../complex-differentiability-at-a-point.md); $\pi$ is a local [biholomorphism](../../../../../../biholomorphism.md) and is onto, since even constant functions provide germs over every point.

The germ space is Hausdorff. Germs over different points are separated by base neighborhoods. For distinct germs over the same point, choose representatives on one small connected disk. If their two sheets met anywhere in that disk, the representatives would agree on an open set and hence everywhere on the disk by the [identity theorem](../../../../../../identity-theorem.md), a contradiction. These sheets thus separate the germs. Together with the allowed second-countability fact, the charts make each component a [Riemann surface](../../../../../../riemann-surfaces.md).

Here “covering in the sense of complex analysis” means this locally biholomorphic, possibly incomplete [analytic germ projection](../../../../../../analytic-germ-projection.md). It does not mean an evenly covered topological [covering map](../../../../../../covering-space.md): an analytic branch can cease to exist at a singularity, so the restriction to a component need not project onto all of $X$.

The evaluation map $E([f]_p)=f(p)$ is [holomorphic](../../../../../../complex-differentiability-at-a-point.md), since on the sheet $\widetilde U_f$ it is just $f$. Starting from one germ, continuation through overlapping disks produces exactly the germs in its connected component. Indeed such continuations give paths in the germ space; conversely, cover a path by finitely many successive sheets to obtain a chain of function elements. Components are path-connected because the surface is locally path-connected. No two distinct germs can be added to that component without being obtainable by continuation. It therefore represents the maximal analytic continuation, or [complete holomorphic function](../../../../../../complete-analytic-function.md), of any of its germs. Conversely every such maximal continuation embeds into the germ space by taking its local germs; completeness makes its image the entire component. These constructions are inverse, giving the requested **bijection between complete holomorphic functions and connected components**, with functions understood up to their natural equivalence as analytic continuations, rather than merely as single-valued functions defined on all of $X$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [22G](../../22g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
