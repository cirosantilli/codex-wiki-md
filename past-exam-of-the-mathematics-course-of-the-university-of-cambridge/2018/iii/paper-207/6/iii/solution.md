<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\pi_A=\mathbb P(T_A<T_B)$, and assume $0<\pi_A<1$ so that both conditional distributions are defined. By [independence](../../../../../../independent-random-variables.md), the joint density of $T_A=u$ and $T_A<T_B$ is $f_A(u)F_B(u)$, whereas the joint density of $T_A=u$ and $T_B<T_A$ is $f_A(u)[1-F_B(u)]$. Normalizing gives

$$
\boxed{f_{T_A\mid T_A<T_B}(u)=\frac{f_A(u)F_B(u)}{\pi_A},\qquad
f_{T_A\mid T_B<T_A}(u)=\frac{f_A(u)[1-F_B(u)]}{1-\pi_A}.}
$$

Both are densities of the latent event time $T_A$. The second is not the density of the observed first event $T_B$ in cases where B wins. Their integrals are 1 by the definitions of $\pi_A$ and its complement.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
