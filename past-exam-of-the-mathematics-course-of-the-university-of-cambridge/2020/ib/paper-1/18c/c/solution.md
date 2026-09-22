<h1 id="18c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The displayed [Rodrigues' formula](../../../../../../rodrigues-formula.md) gives the [Legendre polynomial](../../../../../../legendre-polynomial.md)

$$
q_4(x)=\frac18(35x^4-30x^2+3).
$$

A four-node Gaussian rule is exact through degree $2\cdot4-1=7$. Solving $q_4(x)=0$ first for $x^2$ gives the four nodes

$$
\boxed{c_k\in
\left\{
-\sqrt{\frac{15+2\sqrt{30}}{35}},
-\sqrt{\frac{15-2\sqrt{30}}{35}},
\sqrt{\frac{15-2\sqrt{30}}{35}},
\sqrt{\frac{15+2\sqrt{30}}{35}}
\right\}}.
$$

The rule is not exact for every polynomial of degree eight: its quadrature value on $q_4^2$ is zero because every node is a root of $q_4$, whereas

$$
\boxed{\int_{-1}^1q_4(x)^2\,dx>0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18C](../../18c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
