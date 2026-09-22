# Maximum-area circular segment with fixed arc length and chord

↑ **Parent:** [Planar isoperimetric inequality](planar-isoperimetric-inequality.md)

Fix two attachments a distance $2a$ apart on a straight line and a simple fence of length $2l$ in one half-plane, with $a<l<\pi a/2$. There is a unique $\theta\in(0,\pi/2)$ satisfying $l/a=\theta/\sin\theta$: its derivative has numerator $\sin\theta-\theta\cos\theta>0$, since that numerator starts at zero and has derivative $\theta\sin\theta>0$. A radius-$R$ minor circular arc with half-angle $\theta$ then has the required chord and length. Its graph is $y=\sqrt{R^2-x^2}-\sqrt{R^2-a^2}$, for $-a\leq x\leq a$, and sector-minus-triangle geometry gives the displayed area.

To prove global maximality, attach the complementary major arc of this circle, lying in the opposite half-plane, to any competing fence. The resulting closed curve has perimeter $2l+(2\pi R-2l)=2\pi R$. Its enclosed area is the competitor's area plus a fixed major-segment area. The [planar isoperimetric inequality](planar-isoperimetric-inequality.md) bounds the total by $\pi R^2$, with equality only for a circle. Subtracting that fixed added area proves the minor arc is the unique maximizing shape on the chosen side. The same arc follows from the [Beltrami identity](beltrami-identity.md) for the area-minus-length functional.

## ↑ Ancestors (7)

1. [Planar isoperimetric inequality](planar-isoperimetric-inequality.md)
2. [Isoperimetric inequality](isoperimetric-inequality.md)
3. [Euclidean geometry](euclidean-geometry-split.md)
4. [Geometry and topology](geometry-and-topology-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-1/10/solution.md)
