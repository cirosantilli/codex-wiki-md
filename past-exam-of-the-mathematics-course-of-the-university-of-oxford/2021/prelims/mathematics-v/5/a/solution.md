<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $c>0$ and $L>0$, [D'Alembert's formula](../../../../../../d-alembert-s-formula.md) for the [wave equation](../../../../../../wave-equation-split.md) on the full [real line](../../../../../../real-line.md) is

$$
y(x,t)=\frac{f(x-ct)+f(x+ct)}2+\frac1{2c}\int_{x-ct}^{x+ct}g(s)\,ds.
$$

For the specified initial data, define the cumulative initial-velocity [integral](../../../../../../integral-split.md)

$$
A(s)=\begin{cases}
0,&s\leq-L,\\
(L^2-s^2)/2,&-L\leq s\leq0,\\
(L^2+s^2)/2,&0\leq s\leq L,\\
L^2,&s\geq L.
\end{cases}
$$

Then $\boxed{y(x,t)=[A(x+ct)-A(x-ct)]/(2c)}$. The [initial velocity](../../../../../../initial-velocity.md) jumps at $\pm L$, so the resulting solution is interpreted piecewise classically, or as a weak wave-equation solution across the corresponding [characteristic curves](../../../../../../characteristic-curve.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
