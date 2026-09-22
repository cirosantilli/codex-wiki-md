<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The feasible point $x=(8/5,0,1/5)$ makes the second and third constraints tight; the first has left side two. Its objective is $27/5$.

To prove optimality from first principles, multiply each of the second and third inequalities by $3/5$ and add. For every nonnegative feasible $x$,

$$
3x_1+x_2+3x_3\le3x_1+\frac{12}5x_2+3x_3\le\frac35(5+4)=\frac{27}5.
$$

This is an explicit [weak duality](../../../../../../weak-duality.md) bound, proved here simply by adding inequalities. The displayed point attains it, so

$$
\boxed{\phi(0)=27/5,\qquad x^*=(8/5,0,1/5).}
$$

Equality forces $x_2=0$ and both contributing constraints tight, proving uniqueness as well.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
