# Lens-to-half-plane map through the intersection points

↑ **Parent:** [Möbius transformation](mobius-transformation.md)

A useful way to map a circular lens is to send its two corner points to zero and infinity with a [Möbius transformation](mobius-transformation.md). The two bounding circles then become straight rays, and a suitable power opens their sector into a [half-plane](half-plane.md).

For the lens $|z+1|<\sqrt2$, $|z-1|<\sqrt2$, the corners are $\pm i$. Put $w=(z-i)/(z+i)$, with inverse $z=i(1+w)/(1-w)$. For $w=u+iv$, substitution gives

$$
|z+1|^2-2=\frac{4(u-v)}{|1-w|^2},\qquad |z-1|^2-2=\frac{4(u+v)}{|1-w|^2}.
$$

Thus the image is precisely $u<-|v|$, or $3\pi/4<\arg w<5\pi/4$. Rotation through $-3\pi/4$ followed by squaring gives the displayed [conformal map](conformal-map.md) onto the [upper half-plane](upper-half-plane-complex-analysis.md). The open sector contains no opposite pair, so squaring is injective; it has nonzero [derivative](derivative.md) away from its excluded vertex. These facts also prove bijectivity and conformality, rather than merely identifying boundary images.

## ↑ Ancestors (7)

1. [Möbius transformation](mobius-transformation.md)
2. [Projective linear group](projective-linear-group.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2004/6/solution.md)
