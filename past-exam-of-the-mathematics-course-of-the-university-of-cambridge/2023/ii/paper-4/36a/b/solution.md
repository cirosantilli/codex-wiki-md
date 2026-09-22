<h1 id="36a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Dot the [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md) with $\mathbf E$ and [Faraday's law](../../../../../../faraday-s-law-of-induction.md) with $\mathbf H$:

$$
\mathbf E\cdot\frac{\partial\mathbf D}{\partial t}
=\mathbf E\cdot(\nabla\times\mathbf H)-\mathbf E\cdot\mathbf J,
$$



$$
\mathbf H\cdot\frac{\partial\mathbf B}{\partial t}
=-\mathbf H\cdot(\nabla\times\mathbf E).
$$

Adding and using the vector identity

$$
\nabla\cdot(\mathbf E\times\mathbf H)
=\mathbf H\cdot(\nabla\times\mathbf E)
-\mathbf E\cdot(\nabla\times\mathbf H)
$$

gives

$$
\boxed{
\mathbf E\cdot\frac{\partial\mathbf D}{\partial t}
+\mathbf H\cdot\frac{\partial\mathbf B}{\partial t}
+\nabla\cdot(\mathbf E\times\mathbf H)
=-\mathbf E\cdot\mathbf J}.
$$

This is the local [Poynting theorem](../../../../../../poynting-theorem.md) before specializing the constitutive relations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [36A](../../36a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
