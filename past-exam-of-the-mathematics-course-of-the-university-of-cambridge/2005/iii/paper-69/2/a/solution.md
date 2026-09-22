<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [linear multistep method](../../../../../../linear-multistep-method.md), let $\rho(\zeta)=\zeta^2-12\zeta/7+5/7$ and $\sigma(\zeta)=4\zeta^2/7-2/7$. The [exponential-symbol order criterion for a multistep method](../../../../../../exponential-symbol-order-criterion-for-a-multistep-method.md) compares $\rho(e^z)$ with $z\sigma(e^z)$. Direct expansion gives

$$
\rho(e^z)-z\sigma(e^z)=-\frac{2}{21}z^3+O(z^4).
$$

Equivalently, substitution of exact smooth values into the recurrence leaves $-2h^3y'''(t_n)/21+O(h^4)$, while the coefficients of $1,h,h^2$ cancel. Therefore **$\boxed{\text{order }2}$**; its unnormalized step defect is of order three. The nonzero cubic term excludes order three.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
