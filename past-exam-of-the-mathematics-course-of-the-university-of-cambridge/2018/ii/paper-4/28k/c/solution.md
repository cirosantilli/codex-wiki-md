<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Ignoring the bounded second-order remainder, this is the [linear regression](../../../../../../linear-regression-split.md) model

$$
Y_i-g(x_0)=hZ_i\beta+\varepsilon_i,
\qquad \beta=g'(x_0).
$$

The [ordinary least squares](../../../../../../ordinary-least-squares.md) estimate through the known zero intercept is

$$
\widehat\beta
=\frac{\sum_i(hZ_i)(Y_i-g(x_0))}{\sum_i(hZ_i)^2}
=\boxed{\frac1N\sum_{i=1}^N\frac{Z_i(Y_i-g(x_0))}{h}},
$$

because $Z_i^2=1$. This is the [randomized symmetric finite-difference derivative estimator](../../../../../../randomized-symmetric-finite-difference-derivative-estimator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
