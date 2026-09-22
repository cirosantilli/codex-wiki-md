<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $B$ be the integral operator with kernel $\beta$. Since $Y=BX+\varepsilon$ and the centered error is independent of $X$,

$$
\mathbb E[a_kb_l]
=\mathbb E\!\left[a_k\langle BX,u_l\rangle\right].
$$

Writing $\beta_{lk}=\langle B\phi_k,u_l\rangle$ and using $\mathbb E[a_ka_j]=\lambda_k\mathbf1_{\{j=k\}}$ gives

$$
\mathbb E[a_kb_l]=\lambda_k\beta_{lk}.
$$

Expanding the [function-on-function linear model](../../../../../../function-on-function-linear-model.md) kernel in the product basis therefore yields

$$
\boxed{\beta(t,s)=
\sum_{k=1}^\infty\sum_{l=1}^\infty
\frac{\mathbb E[a_kb_l]}{\lambda_k}\phi_k(s)u_l(t)}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 225](../../../paper-225-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
