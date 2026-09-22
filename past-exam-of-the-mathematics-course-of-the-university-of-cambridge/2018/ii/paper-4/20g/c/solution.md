<h1 id="20g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Now let $n=m=p$ be [prime](../../../../../../prime-number.md) and put $\alpha=\sqrt[p]{p}$ and $A=\mathbb Z[\alpha]$. The [Eisenstein criterion](../../../../../../eisenstein-criterion.md) applied at $p$ gives $[\mathbb Q(\alpha):\mathbb Q]=p$, while the [discriminant of elements of a number field](../../../../../../discriminant-of-elements-of-a-number-field.md) of its power basis is

$$
|\operatorname{disc}(1,\alpha,\ldots,\alpha^{p-1})|
=|N(f'(\alpha))|
=|N(p\alpha^{p-1})|
=p^{2p-1},
$$

where $f(X)=X^p-p$. By the [discriminant-index formula for an integral lattice](../../../../../../discriminant-index-formula-for-an-integral-lattice.md), every prime dividing $[\mathcal O_L:A]$ must therefore be $p$.

Suppose $A\ne\mathcal O_L$. The finite [abelian group](../../../../../../abelian-group.md) $\mathcal O_L/A$ is then a nontrivial [finite p-group](../../../../../../finite-p-group.md), so it contains an element of order $p$. Consequently there is an $x\in\mathcal O_L\setminus A$ such that

$$
x=\frac{g(\alpha)}p,
\qquad
g(X)=\sum_{k=0}^{p-1}c_kX^k\in\mathbb Z[X],
$$

with some $c_k$ not divisible by $p$.

The polynomial $X^p-p$ is Eisenstein, so [total ramification from an Eisenstein polynomial](../../../../../../total-ramification-from-an-eisenstein-polynomial.md) gives a unique prime ideal $P$ above $p$ with normalized [discrete valuation](../../../../../../discrete-valuation.md)

$$
v_P(\alpha)=1,
\qquad
v_P(p)=p.
$$

Let $k_0$ be the least index for which $p\nmid c_{k_0}$. The term $c_{k_0}\alpha^{k_0}$ has valuation $k_0<p$; every earlier term has valuation at least $p$, and every later term with coefficient prime to $p$ has a distinct, larger valuation. The non-Archimedean valuation therefore gives

$$
v_P(g(\alpha))=k_0<p,
\qquad
v_P(x)=k_0-p<0.
$$

This contradicts $x\in\mathcal O_L$, since an [algebraic integer](../../../../../../algebraic-integer.md) has nonnegative valuation at every [prime ideal](../../../../../../prime-ideal.md). Thus $A=\mathcal O_L$, and

$$
\boxed{\mathcal O_L=\mathbb Z[\sqrt[p]{p}]}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20G](../../20g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
