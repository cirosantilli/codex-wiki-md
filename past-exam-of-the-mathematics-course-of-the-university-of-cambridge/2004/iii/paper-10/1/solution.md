<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Adjoin the identity to the bounded multiplicatively closed set, putting $S'=S\cup\{1\}$ and $M=\sup_{s\in S'}\|s\|<\infty$. Define an auxiliary [norm](../../../../../norm.md) on the underlying [Banach space](../../../../../banach-space-split.md) by

$$
p(a)=\sup_{s\in S'}\|sa\|.
$$

The identity ensures $\|a\|\leq p(a)\leq M\|a\|$, so $p$ and the given norm are [equivalent norms](../../../../../equivalent-norms.md). For $s\in S$, closure under multiplication gives $p(sa)\leq p(a)$. Now use the [operator norm](../../../../../operator-norm.md) of left multiplication on this renormed space:

$$
\boxed{\|a\|_1=\sup_{p(b)\leq1}p(ab).}
$$

Left multiplication is faithful, since $a1=a$. It follows that this is a norm, its triangle and scalar laws follow from the operator norm, and $L_{ab}=L_aL_b$ proves submultiplicativity. Also $L_1$ is the identity, so $\|1\|_1=1$, and the contraction property gives $\|s\|_1\leq1$ for every $s\in S$. Finally,

$$
\frac{\|a\|}{M}\leq\frac{p(a)}{p(1)}\leq\|a\|_1\leq M\|a\|.
$$

For the upper bound use $p(ab)\leq M\|a\|\|b\|\leq M\|a\|p(b)$. These bounds prove equivalence and completeness, so this is the required unital [algebra norm](../../../../../algebra-norm.md). This proves [renorming a bounded multiplicative semigroup](../../../../../renorming-a-bounded-multiplicative-semigroup.md); the auxiliary norm is submultiplicative but need not give the identity norm one, which is why the operator norm is used.

The [spectrum of an element](../../../../../spectrum-of-an-element.md) is $\sigma(x)=\{\lambda\in\mathbb C:\lambda1-x\text{ is not invertible in }A\}$. The [spectral radius formula](../../../../../spectral-radius-formula.md) is

$$
\boxed{r(x)=\lim_{m\to\infty}\|x^m\|^{1/m}=\inf_{m\geq1}\|x^m\|^{1/m}.}
$$

If $r(x)<1$, choose $r(x)<q<1$. Eventually $\|x^m\|^{1/m}<q$, hence $\|x^m\|<q^m$. The finitely many earlier powers are bounded too. In particular the power set is bounded; indeed $x^m\to0$ in norm.

For the commuting family, put $d_j=r(x_j)+\varepsilon/2$ and $y_j=x_j/d_j$. Each $r(y_j)<1$, so $M_j=\sup_{m\geq0}\|y_j^m\|<\infty$. Every element of the generated multiplicative semigroup can be reordered as $y_1^{m_1}\cdots y_n^{m_n}$, and its norm is at most $\prod_jM_j$. The first construction therefore gives one equivalent unital algebra norm with $\|y_j\|_0\leq1$ for all $j$, whence

$$
\boxed{\|x_j\|_0\leq r(x_j)+\varepsilon/2<r(x_j)+\varepsilon.}
$$

This is [simultaneous spectral-radius renorming](../../../../../simultaneous-spectral-radius-renorming.md); commutativity is what bounds all mixed products.

For commuting $a,b$, apply this construction to both with error $\varepsilon$. Equivalent algebra norms leave invertibility and spectrum unchanged, and the spectral radius formula gives $r(c)\leq\|c\|_0$. Thus

$$
r(ab)\leq\|a\|_0\|b\|_0<(r(a)+\varepsilon)(r(b)+\varepsilon),\qquad
r(a+b)\leq\|a\|_0+\|b\|_0<r(a)+r(b)+2\varepsilon.
$$

Let $\varepsilon\downarrow0$ to obtain **$r(ab)\leq r(a)r(b)$ and $r(a+b)\leq r(a)+r(b)$**.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
