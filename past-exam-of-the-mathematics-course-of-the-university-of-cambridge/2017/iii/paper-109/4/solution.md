<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md) to prove the [Ray-Chaudhuri–Wilson theorem](../../../../../ray-chaudhuri-wilson-theorem.md). For each $A_i$ define an [intersection polynomial](../../../../../intersection-polynomial.md) over $\mathbb R$,

$$
p_i(x_1,\ldots,x_n)=\prod_{\ell\in L}\left(\sum_{a\in A_i}x_a-\ell\right).
$$

At the [characteristic vector of a set](../../../../../characteristic-vector-of-a-set.md) $A_j$, the inner sum is $|A_i\cap A_j|$. Therefore

$$
p_i(\chi_{A_j})=0\quad(i\ne j),\qquad p_i(\chi_{A_i})=\prod_{\ell\in L}(r-\ell)\ne0.
$$

It follows that the restrictions of $p_1,\ldots,p_m$ to the [uniform layer of the Boolean cube](../../../../../uniform-layer-of-the-boolean-cube.md)

$$
\Omega_r=\{\chi_A:A\subseteq[n],\ |A|=r\}
$$

have [linear independence](../../../../../linear-independence.md): evaluating any vanishing linear combination at each $\chi_{A_j}$ forces its $j$th coefficient to be zero.

Apply [multilinear reduction on the Boolean cube](../../../../../multilinear-reduction-on-the-boolean-cube.md) by replacing each positive power $x_a^t$ in a [monomial](../../../../../monomial.md) with $x_a$. This preserves evaluations on $\{0,1\}^n$ and gives [multilinear polynomials](../../../../../multilinear-polynomial.md) of [polynomial degree](../../../../../degree-of-a-polynomial.md) at most $s$. Counting all [monomials](../../../../../monomial.md) of degrees up to $s$ would give only $\sum_{j=0}^s\binom nj$, which is too weak. Instead use [homogenisation on a uniform layer](../../../../../homogenisation-on-a-uniform-layer.md).

Because $L$ has $s$ distinct integers in $\{0,\ldots,r-1\}$, we have $s\leq r$. For $T\subseteq[n]$ with $|T|=j\leq s$, write $x_T=\prod_{a\in T}x_a$, with $x_\varnothing=1$. On $\Omega_r$,

$$
x_T=\frac{1}{\binom{r-j}{s-j}}\sum_{\substack{S\supseteq T\\|S|=s}}x_S.
$$

Indeed, at $\chi_A$ both sides vanish if $T\nsubseteq A$; otherwise exactly $\binom{r-j}{s-j}$ summands equal $1$. The denominator is positive since $j\leq s\leq r$. Thus every [monomial](../../../../../monomial.md) of degree at most $s$, restricted to $\Omega_r$, lies in the [span](../../../../../linear-span.md) of the $\binom ns$ degree-$s$ [monomials](../../../../../monomial.md). This [vector space](../../../../../vector-space-split.md) consequently has [dimension](../../../../../dimension-vector-space.md) at most $\binom ns$. The [linear independence](../../../../../linear-independence.md) already proved now gives

$$
\boxed{m\leq\binom ns.}
$$

No additional condition such as $r+s\leq n$ is needed: only the spanning upper bound is used, not independence of all degree-$s$ [monomials](../../../../../monomial.md). The argument also covers $s=0$ if empty $L$ is allowed, with the empty product equal to $1$ and at most one member in the [set family](../../../../../set-family.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
