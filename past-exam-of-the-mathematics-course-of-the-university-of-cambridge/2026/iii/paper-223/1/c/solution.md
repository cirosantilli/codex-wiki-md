<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The sample median attains the equivariant upper bound:

$$
\varepsilon^*(\widehat\theta_{\mathrm{med}})
=\frac1n\left\lfloor\frac{n-1}{2}\right\rfloor.
$$

For the Huber estimator, fewer than half the observations cannot overpower the bounded scores of the uncontaminated majority. Evaluating the estimating equation below $x_{(1)}-k$ or above $x_{(n)}+k$ makes every uncontaminated score have the same sign. A contaminating majority can balance these scores arbitrarily far away, so

$$
\varepsilon^*(\widehat\theta_{\mathrm{Hub},k})
=\frac1n\left\lfloor\frac{n-1}{2}\right\rfloor.
$$

A $\gamma$-trimmed mean remains bounded while at most $\lfloor\gamma n\rfloor$ arbitrary observations are removed by each tail trim; one more arbitrarily large replacement survives. Hence

$$
\boxed{\varepsilon^*(\widehat\theta_{\mathrm{trim},\gamma})
=\frac{\lfloor\gamma n\rfloor}{n}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
