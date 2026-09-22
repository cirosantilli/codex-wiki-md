<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

By part (a), $f$ is a bounded [continuous function](../../../../../../continuous-function.md), hence is Borel measurable and integrable for the given [probability measure](../../../../../../probability-measure.md). By part (e), $l\in E'$, and its restriction to the unit ball is also bounded and integrable. For every $u\in U$, the supporting inequality says $f(u)\geq f(x)+l(u)-l(x)$. Taking [expectations](../../../../../../expected-value.md) and using the [barycentre](../../../../../../barycenter.md) hypothesis for this particular $l$ gives

$$
\mathbb E f\geq f(x)+\mathbb E l-l(x)=f(x).
$$

Thus **$\boxed{\mathbb E f\geq f(x)}$**, the [Jensen inequality](../../../../../../jensen-s-inequality.md). This proof only uses the stated weak [barycentre](../../../../../../barycenter.md) identity; a vector-valued integral for the identity map is not needed.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
