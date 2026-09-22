<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Aggregate the individual increments. At an event time $x_i$, their conditional expectation is the number

$$
r_i=\sum_{j=1}^n\mathbf1_{\{x_j\geq x_i\}}
$$

at risk times $dH(x_i)$. Replacing expectation by the observed event increment gives $d\widehat H(x_i)=v_i/r_i$. Thus the estimator is the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md)

$$
\boxed{\widehat H(t)=\sum_{i:x_i\leq t}\frac{v_i}{r_i}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
