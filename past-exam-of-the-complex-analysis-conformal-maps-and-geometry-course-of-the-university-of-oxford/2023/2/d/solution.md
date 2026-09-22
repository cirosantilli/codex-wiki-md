<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the simply connected domain shown in the diagram. A [Riemann mapping theorem](../../../../riemann-mapping-theorem.md) map followed by an [automorphism of the unit disk](../../../../automorphism-of-the-unit-disk.md) sends its marked points to $0$ and $x\in(0,1)$. Split this disc along its real diameter. Map the upper [conformal quadrilateral](../../../../conformal-quadrilateral.md) from [c](../c.md) to a rectangle $[0,w]\times[0,h]$, with $[-1,0]$ and $[x,1]$ as vertical sides and $(0,x)$ as its bottom. The lower half is a second identical rectangle. The full disc is obtained by gluing the two rectangles along their two vertical sides and their bottom sides; the two top sides form the original outer boundary.

In this [doubled rectangle extremal-length duality](../../../../doubled-rectangle-extremal-length-duality.md), loops enclosing both marked bottom corners have shortest flat length $2w$. They must meet both vertical seams, and a closed curve's total horizontal travel is at least $2w$; the doubled horizontal segments attain it. Crosscuts separating the two corners must meet the bottom seam, and run from outer boundary back to outer boundary. Their total vertical travel is at least $2h$, attained by doubled vertical segments. The total flat area is $2wh$.

These flat metrics are extremal, not merely lower bounds. For an arbitrary metric, average the lengths of the doubled horizontal segments over their height and apply the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) to get $L_\rho(\Gamma)^2h\leq2wA_\rho$. Averaging the doubled vertical segments gives $L_\rho(\Gamma^*)^2w\leq2hA_\rho$. Consequently

$$
\boxed{\lambda(\Gamma)=\frac{2w}{h}=2d,\qquad\lambda(\Gamma^*)=\frac{2h}{w}=2d_*,\qquad\lambda(\Gamma)\lambda(\Gamma^*)=4}.
$$

The [conformal metric](../../../../conformal-metric.md) on the doubled rectangles pulls back to an admissible metric on the original punctured domain; the two marked corner points have zero area. Here $\Gamma^*$ consists of crosscuts with endpoints on the outer boundary, as drawn. Boundedness alone, without the illustrated domain topology and the specified curve families, would not justify this construction.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the complex analysis: conformal maps and geometry course of the University of Oxford](../../../split.md)
5. [Complex analysis: conformal maps and geometry course of the University of Oxford](../../../../complex-analysis-conformal-maps-and-geometry-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
