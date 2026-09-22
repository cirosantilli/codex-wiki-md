<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Using $S=N-I$ reduces the system to the [logistic differential equation](../../../../../../logistic-differential-equation.md)

$$
\dot I=\beta I(1-I/N).
$$

Separation of variables and the initial values give

$$
\log\frac{I}{N-I}=\beta t-\log\theta,
\qquad
I(t)=\frac{N}{1+\theta e^{-\beta t}}.
$$

Differentiation yields the incidence

$$
\boxed{\Lambda(t)=\dot I(t)
=\frac{\theta N\beta e^{-\beta t}}
{(1+\theta e^{-\beta t})^2}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
