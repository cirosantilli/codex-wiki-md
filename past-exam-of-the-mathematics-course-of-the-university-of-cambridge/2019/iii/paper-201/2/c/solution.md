<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $V_n=\operatorname{Var}(S_n)=\sum_{m=1}^nv_m$. Then

$$
\begin{aligned}
\mathbb E[S_{n+1}^2-V_{n+1}\mid\mathcal F_n]
&=S_n^2+v_{n+1}-V_n-v_{n+1}\\
&=S_n^2-V_n.
\end{aligned}
$$

Consequently

$$
\boxed{(S_n^2-\operatorname{Var}(S_n))_{n\geq0}
\text{ is a martingale}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
