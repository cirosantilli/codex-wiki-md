<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [Noetherian ring](../../../../../noetherian-ring.md) is a ring whose [ideals](../../../../../ideal.md) satisfy the [ascending chain condition](../../../../../ascending-chain-condition.md); equivalently every [ideal](../../../../../ideal.md) is finitely generated. For the surjective [ring endomorphism](../../../../../ring-endomorphism.md), put $K_j=\ker f^j$. The ascending chain of [ideals](../../../../../ideal.md) $K_1\subseteq K_2\subseteq\cdots$ stabilizes, say $K_m=K_{m+1}$. If $a\in\ker f$, surjectivity of $f^m$ gives $b$ with $f^m(b)=a$. Then $f^{m+1}(b)=0$, so $b\in K_{m+1}=K_m$ and $a=0$. **The [endomorphism](../../../../../endomorphism.md) is therefore injective**, hence a [ring automorphism](../../../../../ring-automorphism.md).

The [nilradical](../../../../../nilradical.md) is the [ideal](../../../../../ideal.md)

$$
N(R)=\sqrt{(0)}=\{a\in R:a^j=0\text{ for some }j\geq1\}.
$$

For example, if $a^u=b^v=0$, the binomial expansion gives $(a+b)^{u+v-1}=0$; multiplication by any ring element also preserves nilpotence. Every [prime ideal](../../../../../prime-ideal.md) contains each [nilpotent element](../../../../../nilpotent.md), since $a^j\in P$ implies $a\in P$. Conversely, if $a$ is not nilpotent, the [multiplicative subset](../../../../../multiplicatively-closed-set.md) $\{1,a,a^2,\ldots\}$ avoids $(0)$. By [Zorn's lemma](../../../../../zorn-s-lemma.md), choose an [ideal](../../../../../ideal.md) maximal among those disjoint from this subset. It is a [prime ideal](../../../../../prime-ideal.md): if $xy\in J$ but neither factor is in $J$, then $J+(x)$ and $J+(y)$ both meet the subset, and multiplying their two witnesses puts a power of $a$ in $J$, a contradiction. This [prime ideal](../../../../../prime-ideal.md) excludes $a$. **Hence**

$$
\boxed{N(R)=\bigcap_{P\in\operatorname{Spec}R}P.}
$$

For the zero ring the empty intersection is the whole ring, as required.

Here is a [finite prime-intersection representation of a radical](../../../../../finite-prime-intersection-representation-of-a-radical.md) argument that does not assume the result. In a [Noetherian ring](../../../../../noetherian-ring.md), suppose some [ideal](../../../../../ideal.md) $J$ has [ideal radical](../../../../../radical-of-an-ideal.md) not expressible as a finite intersection of [prime ideals](../../../../../prime-ideal.md), and choose such a $J$ maximal by the [ascending chain condition](../../../../../ascending-chain-condition.md). It is proper and cannot be prime. Choose $a,b\notin J$ with $ab\in J$. The two larger [ideals](../../../../../ideal.md) $J+(a)$ and $J+(b)$ have finite prime-intersection radicals, and

$$
\sqrt J=\sqrt{J+(a)}\cap\sqrt{J+(b)}.
$$

Indeed, if $x^u\in J+(a)$ and $x^v\in J+(b)$, then $x^{u+v}\in J+(ab)=J$. This contradicts the choice of $J$. Applying the result to $(0)$ proves **that $N(R)$ is the intersection of finitely many [prime ideals](../../../../../prime-ideal.md)**. Empty intersections handle the unit [ideal](../../../../../ideal.md).

For [reducedness of a formal power series ring](../../../../../reducedness-of-a-formal-power-series-ring.md), the inclusion of constants gives one implication: a nonzero [nilpotent element](../../../../../nilpotent.md) of $R$ remains nonzero and nilpotent in $R[[X]]$. For the other, let $R$ be a [reduced ring](../../../../../reduced-ring.md) and take a nonzero [formal power series](../../../../../formal-power-series.md) $F=\sum_{j\geq r}a_jX^j$ with $a_r\ne0$. The coefficient of $X^{mr}$ in $F^m$ is $a_r^m\ne0$, because $R$ is reduced. Thus $F$ is not nilpotent. **Therefore**

$$
\boxed{N(R)=0\quad\Longleftrightarrow\quad N(R[[X]])=0.}
$$

No [Noetherian ring](../../../../../noetherian-ring.md) hypothesis is needed for this argument.

For a [nilradical that is not nilpotent](../../../../../nilradical-that-is-not-nilpotent.md), take

$$
\boxed{R=k[t_1,t_2,\ldots]/(t_1^2,t_2^2,\ldots),\qquad N(R)=(\bar t_1,\bar t_2,\ldots).}
$$

Every element of this [ideal](../../../../../ideal.md) uses finitely many variables and is nilpotent: an element using $s$ variables lies in an [ideal](../../../../../ideal.md) whose $(s+1)$st power is zero. The quotient by this [ideal](../../../../../ideal.md) is the [field](../../../../../field.md) $k$, so it is exactly the [nilradical](../../../../../nilradical.md). Nevertheless $\bar t_1\cdots\bar t_m\ne0$ for every $m$, because the square-free [monomials](../../../../../monomial.md) form a [vector space basis](../../../../../basis.md). Thus $N(R)^m\ne0$ for all $m$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
