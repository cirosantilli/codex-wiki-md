<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Under the independence closure, the mean rightward flux across the bond $(i,i+1)$ is

$$
J_{i+1/2}=k_i^+M_i(1-M_{i+1})
-k_{i+1}^-M_{i+1}(1-M_i).
$$

The mean equation is the discrete conservation law $\dot M_i=J_{i-1/2}-J_{i+1/2}$. Substitution of the rates from part c and Taylor expansion show that the exclusion factors cancel from the symmetric diffusive contribution but remain in the biased contribution:

$$
J=-D\partial_xc+v(x)c(1-c).
$$

Therefore the mean-field [asymmetric simple exclusion process](../../../../../../asymmetric-simple-exclusion-process.md) limit is

$$
\boxed{\partial_tc
=D\partial_x^2c-\partial_x[v(x)c(1-c)].}
$$

The factor $1-c$ is the probability that the destination site is vacant.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
