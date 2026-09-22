<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With complete counts fixed, the likelihood factor for $P_j$ is $P_j^{C_j}(1-P_j)^{U_j}$. As a function of $P_j\in(0,1)$, normalize it to the density of a [Beta distribution](../../../../../../beta-distribution.md) with parameters $C_j+1,U_j+1$. Normalization does not change its maximizing argument. The standard beta-mode formula, when both counts are positive, gives

$$
\boxed{\widehat P_j=\frac{(C_j+1)-1}{(C_j+1)+(U_j+1)-2}
=\frac{C_j}{C_j+U_j}.}
$$

This uses the standard distribution result without differentiating the likelihood, and introducing the normalized beta kernel does not require adopting a Bayesian prior. If only $C_j$ is zero the maximum is at zero; if only $U_j$ is zero it is at one; if both vanish every probability maximizes the constant factor. For the EM M step the same beta-mode argument applies to the expected, possibly noninteger counts, since positive real beta parameters are allowed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
