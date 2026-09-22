<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [projective frame](../../../../projective-frame.md), choose representative vectors $v_1,\ldots,v_{n+1}$ forming a [basis](../../../../basis.md). Express the final point by $\sum c_iv_i$. Every $c_i$ is nonzero, since otherwise some $n+1$ of the given representatives would be dependent. Rescale the first representatives to $c_iv_i$, so the last point is represented by their sum. Do the same for the target frame, with [basis](../../../../basis.md) $w_i$. The [linear map](../../../../linear-map.md) taking each rescaled source [basis](../../../../basis.md) vector to the corresponding target vector induces the required [projective transformation](../../../../projective-linear-transformation.md). For uniqueness, a transformation fixing the first $n+1$ coordinate points is represented by a diagonal matrix. Fixing their sum forces every diagonal entry to agree. It is therefore scalar, giving **a unique [projective transformation](../../../../projective-linear-transformation.md)**.

If three intersection points of the conics lay on a line, Bézout's theorem would force that line to be a component of either nonsingular [conic](../../../../conic-section.md), impossible. Thus the four points form a [projective frame](../../../../projective-frame.md) and can be moved to the three coordinate points and $[1:1:1]$. Vanishing at the coordinate points removes the square terms from each [conic](../../../../conic-section.md) equation; vanishing at the last point gives $a+b+c=0$.

Substitution gives, by direct expansion,

$$
ayz+bzx+cxy=au^2+bv^2+cw^2+(a+b+c)(uv+uw+vw)=au^2+bv^2+cw^2.
$$

The substitution matrix

$$
S=\begin{pmatrix}0&1&1\\1&0&1\\1&1&0\end{pmatrix}
$$

has determinant two, hence is invertible over $\mathbb C$. If the initial frame transformation is represented in the direction old coordinates equal $Q$ times new coordinates, take $P=QS$. Both quadratic forms then have no mixed terms, proving **$P^TAP$ and $P^TBP$ are simultaneously diagonal**. The same argument applies when an individual [conic](../../../../conic-section.md) is reducible but the intersection consists of exactly four distinct points: a line containing three would be a common component, contradicting finiteness of the intersection.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the geometry course of the University of Oxford](../../../split.md)
5. [Geometry course of the University of Oxford](../../../../geometry-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
