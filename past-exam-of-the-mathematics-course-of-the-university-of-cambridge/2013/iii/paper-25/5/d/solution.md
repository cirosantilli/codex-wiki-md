<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At the terminal time, $M_T=e^{i\theta X_T}$, so the martingale from part (c) has terminal value $e^{-\theta^2\langle X\rangle_T/2}$. Its initial value is $M_0$, since $X_0=\langle X\rangle_0=0$. Taking expectations gives

$$
\boxed{\mathbb E e^{i\theta X_T}=\mathbb E e^{-\theta^2\langle X\rangle_T/2}.}
$$

Here $M_0$ may be a nonconstant $\mathcal F_0$-measurable variable; the [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) still gives $\mathbb EM_0=\mathbb E e^{i\theta X_T}$. This [characteristic function under conditionally symmetric martingale increments](../../../../../../characteristic-function-under-conditionally-symmetric-martingale-increments.md) identity relates the [characteristic function](../../../../../../characteristic-function.md) of the terminal martingale to the [Laplace transform of a nonnegative random variable](../../../../../../laplace-transform-of-a-nonnegative-random-variable.md) given by its [quadratic variation](../../../../../../quadratic-variation.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
