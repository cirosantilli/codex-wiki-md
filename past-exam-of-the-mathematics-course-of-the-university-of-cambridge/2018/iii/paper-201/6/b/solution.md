<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $A_n=n^{-1}\sum_{j=1}^nX_j$ and $\varphi(t)=\mathbb E e^{itX_1}$. The given two-sided limit $|f(u)|/u\to0$ implies $|f(u)|/|u|\to0$, so $f(u)=o(|u|)$. For each fixed real $t$, [independence](../../../../../../independent-random-variables.md) and the [characteristic function of a sum of independent variables](../../../../../../characteristic-function-of-a-sum-of-independent-variables.md) give

$$
\mathbb E e^{itA_n}=\left(1+\frac{iat}{n}+f(t/n)\right)^n.
$$

Set $z_n=iat/n+f(t/n)$. For $t\ne0$, $nz_n\to iat$ and $z_n=O(n^{-1})$. The local [Taylor expansion](../../../../../../taylor-expansion.md) of the [complex logarithm](../../../../../../complex-logarithm.md) at $1$ gives

$$
n\log(1+z_n)=nz_n+O(n|z_n|^2)\longrightarrow iat.
$$

Thus $\mathbb E e^{itA_n}\to e^{iat}$; at $t=0$ the identity is immediate. The limit is continuous at zero and is the [characteristic function](../../../../../../characteristic-function.md) of the constant [random variable](../../../../../../random-variable-split.md) $a$. The [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) proves the [weak law from a characteristic-function expansion](../../../../../../weak-law-from-a-characteristic-function-expansion.md):

$$
\boxed{\frac{X_1+\cdots+X_n}{n}\xrightarrow{d}a.}
$$

No [integrability](../../../../../../integrable-random-variable.md) hypothesis has been used. The conclusion is also [convergence in probability](../../../../../../convergence-in-probability.md) by (d)'s [convergence in distribution to a constant implies convergence in probability](../../../../../../convergence-in-distribution-to-a-constant-implies-convergence-in-probability.md). If the word “constant” were to allow complex $a$, the [characteristic function](../../../../../../characteristic-function.md) symmetry $\varphi(-t)=\overline{\varphi(t)}$ forces $a=\overline a$, so it is necessarily real.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
