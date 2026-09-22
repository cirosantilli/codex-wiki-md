<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [four functions theorem](../../../../../../ahlswede-daykin-inequality.md) concerns nonnegative functions $\alpha,\beta,\gamma,\delta$ on the [Boolean lattice](../../../../../../boolean-lattice.md). Its pointwise hypothesis and conclusion are

$$
\alpha(A)\beta(B)\leq\gamma(A\cup B)\delta(A\cap B)\quad\text{for every }A,B,
$$



$$
\boxed{\left(\sum_A\alpha(A)\right)\left(\sum_B\beta(B)\right)\leq\left(\sum_C\gamma(C)\right)\left(\sum_D\delta(D)\right).}
$$

We prove it by eliminating coordinates.

The elementary step is the [two-point four-functions inequality](../../../../../../two-point-four-functions-inequality.md). Suppose $a_ib_j\leq c_{\max(i,j)}d_{\min(i,j)}$ for $i,j\in\{0,1\}$. Put $x=a_0b_1$, $y=a_1b_0$, $M=c_1d_0$, $R=c_0d_1$. Then $x,y\leq M$ and, using the two diagonal bounds,

$$
xy=(a_0b_0)(a_1b_1)\leq(c_0d_0)(c_1d_1)=MR.
$$

If $M>0$, $(M-x)(M-y)\geq0$ yields $x+y\leq M+xy/M\leq M+R$. If $M=0$, both cross terms vanish and the same conclusion holds. Adding the diagonal bounds gives

$$
(a_0+a_1)(b_0+b_1)\leq(c_0+c_1)(d_0+d_1).
$$

For subsets $S,T\subseteq[n-1]$, take $a_i=\alpha(S\cup E_i)$, $b_j=\beta(T\cup E_j)$, $c_i=\gamma((S\cup T)\cup E_i)$ and $d_i=\delta((S\cap T)\cup E_i)$, where $E_0=\varnothing$, $E_1=\{n\}$. The original hypothesis supplies precisely the four inequalities of the elementary step. Therefore the marginal functions

$$
\alpha'(S)=\alpha(S)+\alpha(S\cup\{n\}),
$$

and similarly $\beta',\gamma',\delta'$, satisfy the same pointwise hypothesis on $[n-1]$. Induction, starting with the one-element Boolean lattice on the empty ground set, proves the four functions theorem. This proof includes zero-valued functions without division by zero.

For the [Harris-Kleitman inequality](../../../../../../harris-inequality.md), let $\mathcal F,\mathcal G$ be increasing [set families](../../../../../../set-family.md), meaning they contain every superset of each member. In the theorem take $\alpha=\mathbf1_{\mathcal F}$, $\beta=\mathbf1_{\mathcal G}$, $\gamma=\mathbf1_{\mathcal F\cap\mathcal G}$ and $\delta=1$. If $A\in\mathcal F$ and $B\in\mathcal G$, their union belongs to both increasing families, so the hypothesis holds. Thus, for the uniform probability measure $\mu$ on subsets,

$$
\boxed{\mu(\mathcal F\cap\mathcal G)\geq\mu(\mathcal F)\mu(\mathcal G).}
$$

Mapping every subset to its complement proves the same [Harris-Kleitman inequality](../../../../../../harris-inequality.md) for two decreasing families. An increasing and a decreasing family have the reverse inequality: apply positive correlation to the increasing family and the complement, as a family, of the decreasing one. More generally, increasing nonnegative functions obey the corresponding positive-correlation bound by the same four-functions substitution, since both function values at the union dominate the original values. For an independent-coordinate [product measure](../../../../../../product-measure.md), multiply all four functions by its weight $w$; the identity $w(A)w(B)=w(A\cup B)w(A\cap B)$ preserves the hypothesis and proves the weighted Harris inequality too.

Finally, replace each [intersecting family](../../../../../../intersecting-family.md) $\mathcal A_i$ by its [upward closure of a set family](../../../../../../upward-closure-of-a-set-family.md) $\mathcal U_i$. It is still intersecting: two supersets of intersecting members have nonempty intersection. It contains at most one of each pair $S,S^c$, and hence $|\mathcal U_i|\leq2^{n-1}$. Let $\mathcal D_i$ be the complement of $\mathcal U_i$ as a family. These families are decreasing and have measure at least one half. Their intersections are decreasing too, so repeated [Harris-Kleitman inequality](../../../../../../harris-inequality.md) gives

$$
\mu\left(\bigcap_{i=1}^k\mathcal D_i\right)\geq\prod_{i=1}^k\mu(\mathcal D_i)\geq2^{-k}.
$$

Taking complements and using $\mathcal A_i\subseteq\mathcal U_i$ proves the [union bound for intersecting families](../../../../../../union-bound-for-intersecting-families.md):

$$
\boxed{\left|\bigcup_{i=1}^k\mathcal A_i\right|\leq2^n-2^{n-k}.}
$$

For $k\leq n$, equality is attained by the families of sets containing coordinate $i$, $1\leq i\leq k$. For $k>n$, the displayed real bound implies the integer bound $2^n-1$, which is attained by using the $n$ coordinate families and repeating families as necessary.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
