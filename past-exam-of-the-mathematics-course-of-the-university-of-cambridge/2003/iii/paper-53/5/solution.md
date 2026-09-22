<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [scalar superfield transformation](../../../../../scalar-superfield-transformation.md) is a pullback under a [supertranslation](../../../../../supertranslation.md). Since that transformation mixes $x$ and $\theta$, an odd-coordinate derivative acquires an extra spacetime-derivative term under the coordinate Jacobian. It therefore does not transform as a spinor [superfield](../../../../../superfield.md) merely by differentiating the scalar transformation law. This is [partial derivatives and superfield covariance](../../../../../partial-derivatives-and-superfield-covariance.md).

For explicit signs, split the [Majorana spinor](../../../../../majorana-spinor.md) coordinates into $\theta^\alpha,\bar\theta^{\dot\alpha}$ and use [left Grassmann derivatives](../../../../../left-grassmann-derivative.md). Choose the differential generators

$$
Q_\alpha=\partial_\alpha-i\sigma^m_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_m,
\qquad
\bar Q_{\dot\alpha}=-\bar\partial_{\dot\alpha}
+i\theta^\beta\sigma^m_{\beta\dot\alpha}\partial_m.
$$

For example, $\{\partial_\alpha,\bar Q_{\dot\beta}\}=i\sigma^m_{\alpha\dot\beta}\partial_m$, which is nonzero. Commuting the even [supersymmetry](../../../../../supersymmetry-split.md) variation through $\partial_\alpha$ consequently gives the unwanted translation term.

Replace the ordinary odd-coordinate derivatives by the [supersymmetric covariant derivatives](../../../../../supersymmetric-covariant-derivative.md)

$$
\boxed{D_\alpha=\partial_\alpha+i\sigma^m_{\alpha\dot\beta}\bar\theta^{\dot\beta}\partial_m,
\qquad
\bar D_{\dot\alpha}=-\bar\partial_{\dot\alpha}
-i\theta^\beta\sigma^m_{\beta\dot\alpha}\partial_m.}
$$

The graded product rule cancels the mixed coordinate/derivative terms, giving $\{D,Q\}=\{D,\bar Q\}=\{\bar D,Q\}=\{\bar D,\bar Q\}=0$. Thus $D_\alpha V$ and $\bar D_{\dot\alpha}V$ transform as spinor [superfields](../../../../../superfield.md). Their own mixed algebra is $\{D_\alpha,\bar D_{\dot\beta}\}=-2i\sigma^m_{\alpha\dot\beta}\partial_m$, with equal-chirality [anticommutators](../../../../../anticommutator.md) zero. This covariant differentiation is also what makes a [chiral superfield](../../../../../chiral-superfield.md) constraint $\bar D_{\dot\alpha}Z=0$ [supersymmetry](../../../../../supersymmetry-split.md) invariant. Negating every barred derivative is another convention, but changes the displayed mixed-algebra sign.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [Section A](../section-a.md)
3. [Paper 53](../../paper-53-split.md)
4. [Iii](../../split.md)
5. [2003](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
