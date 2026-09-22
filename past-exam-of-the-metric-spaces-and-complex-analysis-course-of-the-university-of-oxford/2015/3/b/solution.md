<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $S=\sum_{j=0}^{n-1}|a_j|$ and choose $R>\max(1,2S/|a_n|)$. For $|z|>R$, the [triangle inequality](../../../../triangle-inequality.md) gives

$$
\left|\sum_{j=0}^{n-1}a_jz^j\right|\leq S|z|^{n-1}<\frac{|a_n|}{2}|z|^n.
$$

The [reverse triangle inequality](../../../../reverse-triangle-inequality.md) therefore yields

$$
\boxed{|P(z)|>\frac{|a_n|}{2}|z|^n\qquad(|z|>R).}
$$

If $P$ had no [root](../../../../root-of-a-root-system.md), the [function](../../../../function-split.md) $h=1/P$ would be an [entire function](../../../../entire-function.md). The bound just proved makes $h(z)\to0$ as $|z|\to\infty$. On the remaining closed [disk](../../../../disk-mathematics.md), [continuity](../../../../continuous-function.md) and the [extreme value theorem](../../../../extreme-value-theorem.md) make $h$ [bounded](../../../../boundedness.md). Thus $h$ is a bounded [entire function](../../../../entire-function.md), so [Liouville's theorem](../../../../liouville-theorem.md) makes it constant. Its limit at infinity forces that constant to be zero, impossible for a reciprocal.

Consequently **$P$ has a [root](../../../../root-of-a-root-system.md) in $\mathbb C$**. This proves the existence part of the [fundamental theorem of algebra](../../../../fundamental-theorem-of-algebra.md). The invoked [Liouville theorem](../../../../liouville-theorem.md) follows from the [Cauchy integral formula](../../../../cauchy-integral-formula.md): the [Cauchy estimate](../../../../cauchy-estimate.md) $|h'(w)|\leq M/r$ on arbitrarily large [circles](../../../../circle.md) gives $h'=0$ when $h$ is bounded by $M$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
