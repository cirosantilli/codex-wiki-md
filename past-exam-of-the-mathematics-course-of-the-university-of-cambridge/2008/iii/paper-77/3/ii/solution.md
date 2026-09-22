<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md) and [De Boor's algorithm](../../../../../../de-boor-s-algorithm.md) handle nonuniform knots and repeated knots without converting the whole curve. With a tabulated recurrence they require $O(p^2)$ arithmetic after locating the span and use only local control points; a naive recursive basis evaluation wastes work by recomputing the same terms. [De Boor's algorithm](../../../../../../de-boor-s-algorithm.md) evaluates the vector directly using affine combinations. Inside the span these are convex combinations, which makes the geometric construction transparent and avoids the cancellation that can occur in a power-basis representation. Basis evaluation is especially useful when the same knots and parameter are shared by many coordinate functions or many curves, since the weights can be reused.

Precomputed power coefficients followed by [Horner's method](../../../../../../horner-s-method.md) need only $O(p)$ arithmetic per coordinate and are attractive for many evaluations within an unchanged span, particularly for fixed-degree uniform [B-splines](../../../../../../b-spline.md). Coefficient construction has an initial cost, control-point edits require updates to affected spans, and poor scaling of high-degree power coefficients can damage accuracy. Rescaling each span to $[0,1]$ helps. [Bézier curve](../../../../../../bezier-curve.md) extraction has a similar initial conversion cost; [De Casteljau's algorithm](../../../../../../de-casteljau-s-algorithm.md) then gives stable local evaluation, subdivision, a [convex hull](../../../../../../convex-hull.md) bound and geometric flatness tests useful for rendering and intersection.

Subdivision is convenient when an entire polygonal approximation is wanted: refine only where needed and reuse the hierarchy. It is less economical for a single prescribed parameter and requires a geometric error bound before its approximate point can replace exact evaluation. Span lookup itself costs $O(\log n)$ for sorted arbitrary knots, constant work for a uniform interior span, or amortized constant work for an ordered sequence of sample parameters. **Use de Boor for robust general knots, shared basis weights for batches, and precomputed local polynomials or Bézier pieces for repeated interrogation.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
