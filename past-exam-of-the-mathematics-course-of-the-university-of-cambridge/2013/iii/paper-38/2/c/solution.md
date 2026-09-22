<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any feasible primal vector, twice the second constraint plus one third of the third gives

$$
-\frac23x_1+4x_2+3x_3-\frac{17}3x_4\geq\frac{25}3.
$$

Since $x_1,x_4\geq0$,

$$
2x_1+4x_2+3x_3+x_4
=\left(-\frac23x_1+4x_2+3x_3-\frac{17}3x_4\right)
+\frac83x_1+\frac{20}3x_4\geq\frac{25}3.
$$

The vector $(0,11/6,1/3,0)$ is feasible and attains this bound. **It is optimal**, by this direct inequality proof of [weak duality](../../../../../../weak-duality.md), without assuming the [simplex method](../../../../../../simplex-method.md) or a duality theorem. Equality forces $x_1=x_4=0$ and both positively weighted constraints tight, so it also proves uniqueness.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
