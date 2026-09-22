<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [parametric surface interrogation](../../../../../../parametric-surface-interrogation.md) interface must specify its parameter domain, patch boundaries, trimming restrictions and any exceptional or singular points. It must evaluate $S(u,v)$ and the available [derivatives](../../../../../../derivative.md), in particular $S_u,S_v$ for [tangent vectors](../../../../../../tangent-vector.md) and

$$
n=\frac{S_u\times S_v}{\|S_u\times S_v\|}
$$

for the oriented [normal vector](../../../../../../normal-vector.md) where the denominator is nonzero. Second derivatives $S_{uu},S_{uv},S_{vv}$ are needed when the code requests curvature or second-order geometric error estimates; higher derivatives depend on the enquiry. The interface must report where these quantities exist, rather than assign an artificial normal at a singular parameter point.

Global searches also need subdivision into equivalent restricted patches, certified [bounding volumes](../../../../../../bounding-volume.md) and a geometric approximation/error bound. These support intersection isolation, pruning and tolerance-controlled meshing. A single point-evaluation routine cannot guarantee a global search because it may miss remote branches or features between samples. Adjacent-patch topology and consistent orientation are needed to join results and interpret the represented surface.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
