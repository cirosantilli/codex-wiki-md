<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $Z(\alpha)=\sum_xQ(x)^\alpha$ and $\ell(x)=\log_2Q(x)$. Then

$$
H(Q_\alpha)=-\alpha\mathbb E_\alpha\ell+\log_2Z(\alpha).
$$

Differentiation of this [exponential family](../../../../../../exponential-family-split.md) gives

$$
\frac d{d\alpha}\mathbb E_\alpha\ell
=(\ln2)\operatorname{Var}_\alpha(\ell),
\qquad
\frac d{d\alpha}\log_2Z=\mathbb E_\alpha\ell.
$$

The first-order terms cancel, leaving

$$
\frac d{d\alpha}H(X_\alpha)
=-\alpha(\log_e2)
\operatorname{Var}(\log_2Q(X_\alpha)).
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
