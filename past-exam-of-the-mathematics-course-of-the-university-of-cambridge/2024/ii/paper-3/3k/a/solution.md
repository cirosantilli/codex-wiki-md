<h1 id="3k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Reed-Muller code](../../../../../../reed-muller-code.md) is spanned by the evaluation [vectors](../../../../../../vector.md) of the square-free monomials

$$
\prod_{i\in I}x_i,\qquad |I|\leq r,
$$

form a [basis](../../../../../../basis.md): every Boolean [function](../../../../../../function-split.md) has a unique algebraic normal form, so the monomials remain independent after evaluation on $\mathbb F_2^d$. Thus

$$
\dim\operatorname{RM}(d,r)=\sum_{j=0}^r\binom dj.
$$

Induction using the decomposition $(u,u+v)$, with $u\in\operatorname{RM}(d-1,r)$ and $v\in\operatorname{RM}(d-1,r-1)$, gives the lower bound $2^{d-r}$ for every nonzero weight. The monomial $x_1\cdots x_r$ attains it, so the minimum distance is

$$
\boxed{d_{\min}=2^{d-r}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3K](../../3k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
