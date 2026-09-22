<h1 id="2/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $P_k$ be orthogonal projection onto the column space of $X_k$, and let $\mu$ be the true mean. Then

$$
\operatorname{RSS}_k=\|(I-P_k)Y\|^2
\sim\chi^2_{n-p_k}(\lambda_k),
\qquad
\lambda_k=\|(I-P_k)\mu\|^2.
$$

Up to a common constant,

$$
\operatorname{AIC}_k\sim\chi^2_{n-p_k}(\lambda_k)+2p_k,
\quad
\operatorname{BIC}_k\sim\chi^2_{n-p_k}(\lambda_k)+p_k\log n.
$$

The true model has $p_k=p^*$ and $\lambda_k=0$; every other candidate has $p_k>p^*$ and $\lambda_k\geq0$. Its excess expected AIC is $\lambda_k+p_k-p^*>0$, while its excess expected BIC is $\lambda_k+(\log n-1)(p_k-p^*)>0$ when $n>e$. Thus either minimum expected criterion selects the true model.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Paper 218](../../../../paper-218-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
