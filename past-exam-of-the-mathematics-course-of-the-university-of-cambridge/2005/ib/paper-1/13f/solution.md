<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

Use the [Möbius transformation](../../../../../mobius-transformation.md) $t=(z-1)/(z+1)$, the [principal square root](../../../../../principal-square-root-of-a-complex-number.md) $s=\sqrt t$ with $\Re s>0$, and then $w=(s-1)/(s+1)$. The resulting [conformal map](../../../../../conformal-map.md) is

$$
\boxed{w(z)=\frac{\sqrt{(z-1)/(z+1)}-1}{\sqrt{(z-1)/(z+1)}+1}}.
$$

All branches here are single-valued: the inverse $z=(1+t)/(1-t)$ shows that the deleted segment corresponds to the nonpositive real axis. However, the exact first image is

$$
t(\mathbb C\setminus[-1,1])
=\bigl(\mathbb C\setminus(-\infty,0]\bigr)\setminus\{1\},
$$

since $t=1$ would require a source point at infinity. Thus the next image is $\{\Re s>0\}\setminus\{1\}$, and

$$
\boxed{w(\mathbb C\setminus[-1,1])=\{0<|w|<1\}}.
$$

The strict inequality $|w|<1$ follows from $|s+1|^2-|s-1|^2=4\Re s>0$. None of the component derivatives vanishes. For completeness the inverse on this punctured disk is

$$
z=-\frac12(w+w^{-1}).
$$

Given $0<|w|<1$, the inverse Cayley transform has positive real part, and reversing the three maps proves both injectivity and surjectivity onto this exact image.

This distinction matters for interpreting the printed request. The displayed function is a [conformal map](../../../../../conformal-map.md) into the unit disk, but **no conformal bijection from the specified plane domain onto the full unit disk exists**. To prove the obstruction, the loop $z=2e^{i\theta}$ surrounds $0$, a point outside the domain, with [winding number](../../../../../winding-number.md) $1$. A contraction within the source would remain in $\mathbb C\setminus\{0\}$ and preserve [winding number](../../../../../winding-number.md), whereas a constant loop has [winding number](../../../../../winding-number.md) $0$. Hence the source is not [simply connected](../../../../../simply-connected-space.md); a disk is [simply connected](../../../../../simply-connected-space.md), as straight-line contraction shows, and a conformal bijection is a [homeomorphism](../../../../../homeomorphism.md).

The hinted construction becomes a bijection onto the full disk if the source is instead $\widehat{\mathbb C}\setminus[-1,1]$, including infinity on the [Riemann sphere](../../../../../riemann-sphere.md). Near infinity, $w(z)=-1/(2z)+O(z^{-3})$, so the map extends with $w(\infty)=0$ and nonzero derivative in the coordinate $1/z$. This is the precise filled-in version of the [conformal map of a segment complement to a punctured disk](../../../../../conformal-map-of-a-segment-complement-to-a-punctured-disk.md).

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
