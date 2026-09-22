<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the distribution $R$ associated with the code in part b. Since $2^{L(x)}=(KR(x))^{-1}$,

$$
\mathbb E_P2^{\rho L(X)}
=K^{-\rho}\sum_xP(x)R(x)^{-\rho}
\geq\sum_xP(x)R(x)^{-\rho}.
$$

For $\alpha=1/(1+\rho)$, [Holder inequality](../../../../../../holder-inequality.md), equivalently the indicated [Jensen inequality](../../../../../../jensen-s-inequality.md), gives

$$
\sum_xP(x)R(x)^{-\rho}
\geq\left(\sum_xP(x)^\alpha\right)^{1/\alpha}.
$$

Therefore

$$
\boxed{\frac1\rho\log_2\mathbb E2^{\rho L(X_1^n)}
\geq\frac{1+\rho}{\rho}
\log_2\sum_xP_n(x)^{1/(1+\rho)}
=H_\alpha(X_1^n).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
