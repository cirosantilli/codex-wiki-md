<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Suppose $S$ is a [saturated multiplicative subset](../../../../../../saturated-multiplicative-subset.md), and take $a\notin S$. The principal [ideal](../../../../../../ideal.md) $(a)$ is disjoint from $S$: otherwise $ra\in S$ would force $a\in S$. The [prime ideal avoiding a multiplicative subset](../../../../../../prime-ideal-avoiding-a-multiplicative-subset.md) argument from Question 1 extends $(a)$ to a [prime ideal](../../../../../../prime-ideal.md) $P_a$ disjoint from $S$. Thus every point of the complement belongs to such a [prime ideal](../../../../../../prime-ideal.md), and

$$
\boxed{R\setminus S=\bigcup_{P\cap S=\varnothing}P.}
$$

If $S=R$, this is the empty union.

Conversely suppose $R\setminus S$ is a union of [prime ideals](../../../../../../prime-ideal.md). If $xy\in S$ and $x\notin S$, some [prime ideal](../../../../../../prime-ideal.md) in that union contains $x$, and hence $xy$, a contradiction. The same holds for $y$. Thus **The [saturated complement as a union of prime ideals](../../../../../../saturated-complement-as-a-union-of-prime-ideals.md) characterization holds**.

For [units with no finite prime-union complement](../../../../../../units-with-no-finite-prime-union-complement.md), take

$$
\boxed{R=\mathbb Z,\qquad S=\mathbb Z^\times=\{-1,1\}.}
$$

Products of units are units, and a product is a unit only if both factors are units, so $S$ is a [saturated multiplicative subset](../../../../../../saturated-multiplicative-subset.md). Every nonunit integer lies in some $(p)$ with $p$ a positive prime, giving $\mathbb Z\setminus S=\bigcup_p(p)$. If finitely many [prime ideals](../../../../../../prime-ideal.md) sufficed, discard any $(0)$ and write the others as $(p_1),\ldots,(p_r)$. A prime $\ell$ outside this finite list belongs to none of them but is a nonunit, a contradiction. There is always such an $\ell$: a prime divisor of $p_1\cdots p_r+1$ is outside the list.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
