<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $N_m=|\{i:c_i=m\}|$. The label likelihood for the [mixture weights](../../../../../../../mixture-weight.md) is proportional to $\prod_{m=1}^3\pi_m^{N_m}$. Multiplication by the $\operatorname{Dirichlet}(\alpha_1,\alpha_2,\alpha_3)$ density and [Dirichlet-multinomial conjugacy](../../../../../../../dirichlet-multinomial-conjugacy.md) gives

$$
(\pi_1,\pi_2,\pi_3)\mid y,c,f
\sim\operatorname{Dirichlet}(\alpha_1+N_1,\alpha_2+N_2,\alpha_3+N_3).
$$

Conditional on the labels, the observations and component means provide no further information about $\pi$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
