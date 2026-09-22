<h1 id="section-a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the intended collocation weights, interpolation makes the associated [quadrature rule](../../../../../../../quadrature-rule.md) exact for every polynomial of degree at most one, so the method has order at least two. It has order at least three precisely when the node polynomial is orthogonal to constants:

$$
0=\int_0^1(t-\alpha)(t-1)\,dt
=\frac\alpha2-\frac16.
$$

Thus

$$
\boxed{p=3\text{ when }\alpha=\frac13,
\qquad p=2\text{ for every other }\alpha\ne1.}
$$

At $\alpha=1/3$ this is the two-stage [Radau IIA method](../../../../../../../radau-iia-method.md). Since one node is fixed at the endpoint, no value of $\alpha$ makes the two-node quadrature exact through degree three, so order four cannot occur.

For completeness, the tableau exactly as printed has order zero when $\alpha\ne1/2$, since $b^T\mathbf1\ne1$. At $\alpha=1/2$ the two signs coincide because the second weight vanishes, and the resulting method has order two.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Section A](../../../section-a.md)
4. [Paper 341](../../../../paper-341-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
