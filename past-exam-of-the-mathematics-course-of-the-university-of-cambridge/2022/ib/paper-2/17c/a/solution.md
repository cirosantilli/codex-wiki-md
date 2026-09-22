<h1 id="17c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Writing $f,f',f''$ at $y_n$, the implicit stage has the expansion

$$
k_2=f+h f'f+h^2\left(a(f')^2f+\frac12f''f^2\right)+O(h^3).
$$

Thus one step is

$$
y_{n+1}=y_n+hf+\frac{h^2}{2}f'f
+h^3\left(\frac a2(f')^2f+\frac14f''f^2\right)+O(h^4).
$$

The exact [Taylor expansion](../../../../../../taylor-theorem.md) has third-order term

$$
\frac{h^3}{6}\bigl((f')^2f+f''f^2\bigr).
$$

The coefficients agree through order two for every real $a$, while the $f''f^2$ coefficient prevents order three for any $a$. Hence the [order of a Runge-Kutta method](../../../../../../order-of-a-runge-kutta-method.md) is

$$
\boxed{2\quad\text{for every }a\in\mathbb R}.
$$

(The linear special case has one extra matched term when $a=1/3$, but the order for general nonlinear equations remains two.)

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17C](../../17c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
