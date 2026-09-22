<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

For each $x\in X$, the product $\prod_{i=1}^m(1-g_i(x))$ is $1$ precisely outside every $X_i$, and is $0$ otherwise. It is therefore the [indicator function](../../../../../indicator-function.md) of $Y$. Expanding the finite product gives

$$
\prod_{i=1}^m(1-g_i(x))
=\sum_{S\subseteq\{1,\ldots,m\}}(-1)^{|S|}\prod_{i\in S}g_i(x).
$$

Multiply by $f(x)$ and sum over the finite [set](../../../../../set-split.md) $X$. The product of [indicator functions](../../../../../indicator-function.md) is the [indicator function](../../../../../indicator-function.md) of the corresponding intersection, so

$$
\sum_{x\in Y}f(x)
=\sum_{S\subseteq\{1,\ldots,m\}}(-1)^{|S|}
\sum_{x\in\bigcap_{i\in S}X_i}f(x).
$$

Here the empty intersection is $X$, and the empty product is $1$. Grouping the [subsets](../../../../../subset.md) $S$ by their [cardinality](../../../../../cardinality.md) gives the requested [weighted inclusion-exclusion principle](../../../../../weighted-inclusion-exclusion-principle.md), with no contribution for $r>m$.

Let $\mathcal P$ be the finite [set](../../../../../set-split.md) of distinct [prime factors](../../../../../prime-factor.md) of $n$, and work in $\{0,\ldots,n-1\}$. For $S\subseteq\mathcal P$ put $d_S=\prod_{p\in S}p$, including $d_\varnothing=1$. Then $d_S\mid n$, and an [integer](../../../../../integer.md) belongs to every $X_p$ for $p\in S$ exactly when it is a multiple of $d_S$. Thus the intersection has size $n/d_S$. The complement consists precisely of the residues [coprime](../../../../../coprime-integers.md) to $n$. Using weight $1$ gives

$$
\boxed{\varphi(n)=\sum_{S\subseteq\mathcal P}(-1)^{|S|}\frac n{d_S}
=n\prod_{p\mid n}\left(1-\frac1p\right).}
$$

This proves the product formula for the [Euler totient function](../../../../../euler-totient-function.md) without requiring $n$ to be squarefree.

For the weight $f(x)=x$, the sum over the multiples of any divisor $d$ in this interval is

$$
\sum_{j=0}^{n/d-1}dj
=\frac{n^2}{2d}-\frac n2.
$$

The [weighted inclusion-exclusion principle](../../../../../weighted-inclusion-exclusion-principle.md) therefore gives

$$
\sum_{\substack{0<x<n\\(x,n)=1}}x
=\frac{n^2}{2}\sum_{S\subseteq\mathcal P}\frac{(-1)^{|S|}}{d_S}
-\frac n2\sum_{S\subseteq\mathcal P}(-1)^{|S|}.
$$

Since $n>1$, $\mathcal P$ is nonempty and the last sum is $(1-1)^{|\mathcal P|}=0$. The first factors as before, giving

$$
\boxed{\sum_{\substack{0<x<n\\(x,n)=1}}x
=\frac{n^2}{2}\prod_{p\mid n}\left(1-\frac1p\right)
=\frac{n\varphi(n)}2.}
$$

This [sum of reduced residues](../../../../../sum-of-reduced-residues.md) also follows by pairing the [bijection](../../../../../bijection.md) $x\mapsto n-x$; at $n=2$ its sole fixed residue causes no problem because the sum of both copies still equals $n\varphi(n)$.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
