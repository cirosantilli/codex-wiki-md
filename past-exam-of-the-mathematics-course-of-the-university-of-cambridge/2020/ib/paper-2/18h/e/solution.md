<h1 id="18h/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Full column rank of $X$ makes $X^T:\mathbb R^n\to\mathbb R^p$ surjective. Given $x\in\mathbb R^p$, choose $u$ with $x=X^Tu$. The fitted values for the unrestricted and restricted regressions are

$$
X\widehat\beta=PY,
\qquad
X\widetilde\beta=P_0Y.
$$

Therefore

$$
x^T\widehat\beta=u^TPY,
\qquad
x^T\widetilde\beta=u^TP_0Y.
$$

Using $\operatorname{cov}(Y)=\sigma^2I_n$ and idempotence of the projections,

$$
\operatorname{var}(x^T\widehat\beta)
=\sigma^2u^TPu,
\qquad
\operatorname{var}(x^T\widetilde\beta)
=\sigma^2u^TP_0u.
$$

Part (d) now gives

$$
\boxed{\operatorname{var}(x^T\widetilde\beta)
\le\operatorname{var}(x^T\widehat\beta)}.
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [18H](../../18h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
