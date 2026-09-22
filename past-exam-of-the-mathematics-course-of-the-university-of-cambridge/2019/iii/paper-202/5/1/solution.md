<h1 id="5/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [simple predictable process](../../../../../../simple-predictable-process.md) has the form

$$
H_s=\sum_{i=0}^{n-1}\xi_i\mathbf1_{(t_i,t_{i+1}]}(s),
$$

where each bounded $\xi_i$ is $\mathcal F_{t_i}$-measurable. Define

$$
(H\mathbin\cdot B)_t
=\sum_i\xi_i(B_{t\wedge t_{i+1}}-B_{t\wedge t_i}).
$$

Independent centered Brownian increments show directly by conditioning that this is a martingale. The same conditional expansion, using $\mathbb E[(B_v-B_u)^2\mid\mathcal F_u]=v-u$, shows that

$$
\boxed{(H\mathbin\cdot B)_t^2-\int_0^tH_s^2ds
\text{ is a martingale}.}
$$

## ↑ Ancestors (11)

1. [1](../1.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
