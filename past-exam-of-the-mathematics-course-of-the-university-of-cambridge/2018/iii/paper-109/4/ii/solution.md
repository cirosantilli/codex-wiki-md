<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Work in the [prime field](../../../../../../prime-field.md) $\mathbb F_p$ and set $r=p-1$. We will choose $a_p=0$, use the other $a_i$ to enumerate $\mathbb F_p^*$, and ensure that the first $r$ values of $c_i=a_i+b_i$ are distinct. The zero-sum condition will then force the last value to be the missing field element.

Consider the [polynomial](../../../../../../polynomial-split.md)

$$
P(x_1,\ldots,x_r)=\prod_{1\leq i<j\leq r}(x_j-x_i)(x_j+b_j-x_i-b_i).
$$

It has [total degree of a polynomial](../../../../../../total-degree-of-a-polynomial.md) $r(r-1)$. Its terms of highest total degree form the [homogeneous polynomial](../../../../../../homogeneous-polynomial.md) given by the square of the [Vandermonde determinant](../../../../../../vandermonde-determinant.md), $\Delta(x)^2=\prod_{i<j}(x_j-x_i)^2$. For [coefficient extraction](../../../../../../coefficient-extraction.md) we need the coefficient of $\prod_i x_i^{r-1}$; lower-degree terms of $P$ cannot contribute to it.

Apply the [Dyson constant-term identity](../../../../../../dyson-constant-term-identity.md) from part (i) in $r$ variables, with every exponent equal to one. Pairing its factors for $i,j$ gives

$$
\prod_{i\ne j}\left(1-\frac{x_i}{x_j}\right)=(-1)^{\binom r2}\frac{\Delta(x)^2}{\prod_i x_i^{r-1}}.
$$

The [constant term](../../../../../../constant-term.md) is $r!$. Thus the desired coefficient is

$$
\left[\prod_i x_i^{r-1}\right]P=(-1)^{\binom r2}r!\ne0\quad\text{in }\mathbb F_p,
$$

since none of $1,\ldots,p-1$ is zero in the [prime field](../../../../../../prime-field.md).

For completeness, the coefficient form of the [Combinatorial Nullstellensatz](../../../../../../combinatorial-nullstellensatz.md), also called the [Alon-Tarsi lemma](../../../../../../alon-tarsi-lemma.md), says that if $\deg P\leq\sum_i d_i$ and each finite set $S_i$ in a [field](../../../../../../field.md) has size $d_i+1$, then

$$
\left[\prod_i x_i^{d_i}\right]P=\sum_{s\in S_1\times\cdots\times S_r}\frac{P(s)}{\displaystyle\prod_{i=1}^r\prod_{t\in S_i\setminus\{s_i\}}(s_i-t)}.
$$

To justify this formula, the univariate [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) coefficient functional kills powers below $d_i$ and takes the value one on $x_i^{d_i}$. Apply the product of these functionals to each [monomial](../../../../../../monomial.md) of $P$. Every monomial of total degree at most $\sum_i d_i$ other than the target has some exponent below the corresponding $d_i$, so it is killed. The target survives with coefficient one. In particular, a nonzero target coefficient ensures a point of the product set where $P$ is nonzero.

Use $S_i=\mathbb F_p^*$ and $d_i=r-1$ for every $i$. The degree bound holds with equality, so there is $(a_1,\ldots,a_r)\in(\mathbb F_p^*)^r$ with $P(a)\ne0$. Its first factors ensure that the $a_i$ are distinct; its second factors ensure that $c_i=a_i+b_i$, $1\leq i\leq r$, are distinct. With $a_p=0$, the $a_i$ enumerate the whole [prime field](../../../../../../prime-field.md).

Let $q$ be the unique field element missing from $c_1,\ldots,c_r$, and write $T=\sum_{x\in\mathbb F_p}x$. Since $\sum_i b_i=0$,

$$
\sum_{i=1}^r c_i=\sum_{i=1}^r a_i+\sum_{i=1}^r b_i=T-b_p.
$$

The same sum is $T-q$, hence $q=b_p$. Taking $c_p=b_p=a_p+b_p$ completes the enumeration. We have proved [zero-sum sequences as differences of permutations of a prime field](../../../../../../zero-sum-sequences-as-differences-of-permutations-of-a-prime-field.md):

$$
\boxed{\{a_1,\ldots,a_p\}=\{c_1,\ldots,c_p\}=\mathbb F_p,\qquad c_i-a_i=b_i\text{ for every }i.}
$$

No distinctness assumption on the $b_i$ was used. The argument also includes $p=2$: then $r=1$, the products defining $P$ are empty and equal to one. Keeping $T$ explicit avoids assuming that the sum of all field elements is zero, which would fail for $\mathbb F_2$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
