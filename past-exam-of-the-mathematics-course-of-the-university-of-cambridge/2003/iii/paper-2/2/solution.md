<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $A=R[[X]]$, and let $J$ be any ideal of this [formal power series ring](../../../../../formal-power-series.md). For $d\ge0$ define an ideal of $R$ by

$$
L_d=\{a\in R:\text{some }f\in J\cap X^dA\text{ has coefficient }a\text{ at }X^d\}.
$$

Multiplication by $X$ shows $L_d\subseteq L_{d+1}$. Since $R$ is [Noetherian](../../../../../noetherian-ring.md), this chain stabilizes at some $d=N$, and each $L_d$ is finitely generated. For every $0\le d\le N$, choose finitely many series $f_{d,j}\in J\cap X^dA$ whose degree-$d$ coefficients generate $L_d$.

Given $f\in J$, cancel its degree-zero coefficient using the $f_{0,j}$, then its degree-one coefficient using the $f_{1,j}$, and so on. At a degree $d\ge N$, use $X^{d-N}f_{N,j}$. Each residual remains in $J$ and has zero coefficients below the next cancellation degree. For each of the finitely many chosen $f_{d,j}$, accumulate its multiplier into a [formal power series](../../../../../formal-power-series.md) $h_{d,j}$. The higher-degree increments of these multipliers converge coefficientwise. At every degree the cancellation procedure gives the exact coefficient identity, so

$$
f=\sum_{d=0}^N\sum_jh_{d,j}f_{d,j}.
$$

Thus the finitely many lifts generate $J$ as an actual ideal. No assumption that $J$ is closed has been used. This proves [Noetherianity of formal power series rings](../../../../../noetherianity-of-formal-power-series-rings.md):

$$
\boxed{R[[X]]\text{ is Noetherian}.}
$$

Iterating the argument proves the assertion for $R[[X_1,\ldots,X_s]]$, which is naturally the iterated [formal power series ring](../../../../../formal-power-series.md).

For a surjective module map $f:M\to N$, define the [adic completion of a module](../../../../../adic-completion-of-a-module.md) by

$$
\widehat M=\varprojlim_{r\ge1}M/I^rM,\qquad
\widehat N=\varprojlim_{r\ge1}N/I^rN.
$$

Take $\widehat n\in\widehat N$ and choose representatives $n_r\in N$ for its components. Compatibility says $n_{r+1}-n_r\in I^rN$. Choose $m_1$ with $f(m_1)=n_1$. If $f(m_r)=n_r$, surjectivity gives $f(I^rM)=I^rN$, so choose $\delta_r\in I^rM$ with $f(\delta_r)=n_{r+1}-n_r$ and put $m_{r+1}=m_r+\delta_r$. The classes of $m_r$ modulo $I^rM$ are compatible and map to the chosen components of $\widehat n$. Hence

$$
\boxed{\widehat M\longrightarrow\widehat N\text{ is surjective}.}
$$

This [surjectivity on adic completions](../../../../../surjectivity-on-adic-completions.md) does not require finite generation of $M$ or $N$. The compatibility of the lifts is the point; independent lifts of the finite-level classes would not suffice.

Since $R$ is [Noetherian](../../../../../noetherian-ring.md), write $I=(a_1,\ldots,a_s)$. Define a ring homomorphism

$$
\Phi:R[[X_1,\ldots,X_s]]\longrightarrow\widehat R,
\qquad X_i\longmapsto a_i.
$$

Modulo $I^r$, evaluating a series requires only its finitely many terms of total degree below $r$. These evaluations commute with the reduction maps, and define $\Phi$ without needing the original ring to be complete or separated.

To prove surjectivity, begin with $\widehat b\in\widehat R$. Choose $b_0\in R$ matching its component modulo $I$. After terms of total degree below $r$ have been chosen, their evaluation differs from $\widehat b$ at level $R/I^{r+1}$ by a class in $I^r/I^{r+1}$. This class is an $R$-linear combination of the monomials $a^\alpha$ with $|\alpha|=r$. Choose the corresponding homogeneous degree-$r$ polynomial $p_r(X)$ as the next term. Then the series $b_0+\sum_{r\ge1}p_r(X)$ evaluates to $\widehat b$ at every level. This proves the [power-series presentation of an adic completion](../../../../../power-series-presentation-of-an-adic-completion.md), and therefore

$$
\boxed{\widehat R\cong R[[X_1,\ldots,X_s]]/\ker\Phi\text{ is Noetherian}.}
$$

A quotient of a [Noetherian ring](../../../../../noetherian-ring.md) is Noetherian, since its ideals correspond to ideals containing the kernel. The cases $I=0$ and $I=R$ give $\widehat R=R$ and $\widehat R=0$, respectively, and satisfy the conclusion as well.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
