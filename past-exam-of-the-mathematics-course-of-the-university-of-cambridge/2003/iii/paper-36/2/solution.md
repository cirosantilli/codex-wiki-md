<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [finite field](../../../../../finite-field.md) is a [field](../../../../../field.md) with finitely many elements. Its characteristic is the least positive integer $p$ for which $p\cdot1=0$; such an integer exists because the additive group is finite. If $p=ab$ with $1<a,b<p$, then $(a\cdot1)(b\cdot1)=0$ although neither factor is zero, impossible in a [field](../../../../../field.md). Hence $p$ is prime, and the multiples of $1$ form its [prime field](../../../../../prime-field.md) $\mathbb F_p$. The whole [field](../../../../../field.md) is a finite-dimensional [vector space](../../../../../vector-space-split.md) over this subfield, say of [dimension](../../../../../dimension-vector-space.md) $s\geq1$, so its cardinality is $p^s$. Thus **$q=p^s$ and its characteristic is $p$**.

For existence, let $K$ be a [splitting field](../../../../../splitting-field.md) over $\mathbb F_p$ of $P(T)=T^{p^s}-T$. Since $P'(T)=-1$, it has exactly $p^s$ distinct roots. Its root set $F$ contains $0,1$ and is closed under addition and multiplication, because iterated [Frobenius endomorphism](../../../../../frobenius-endomorphism.md) gives

$$
(a+b)^{p^s}=a^{p^s}+b^{p^s},\qquad (ab)^{p^s}=a^{p^s}b^{p^s}.
$$

It is also closed under additive inverses, and for $a\ne0$, $(a^{-1})^{p^s}=(a^{p^s})^{-1}=a^{-1}$. Thus $F$ is a [field](../../../../../field.md) with exactly $p^s$ elements. Since it contains every root, it is the entire [splitting field](../../../../../splitting-field.md). This proves existence.

For uniqueness, let $L$ be any [field](../../../../../field.md) with $p^s$ elements. Its nonzero multiplicative group has order $p^s-1$, so [Lagrange's theorem](../../../../../lagrange-s-theorem.md) gives $a^{p^s}=a$ for every $a\in L$, including zero. Hence $L$ is a [splitting field](../../../../../splitting-field.md) of the same [polynomial](../../../../../polynomial-split.md). Here is the embedding argument giving uniqueness, rather than merely invoking it by name. Extend the identity on $\mathbb F_p$ from one root at a time. If an embedding is already defined on $E$ and a new root $\alpha$ has [minimal polynomial of an algebraic element](../../../../../minimal-polynomial-of-an-algebraic-element.md) $h$ over $E$, the transported [polynomial](../../../../../polynomial-split.md) divides $P$ and therefore has a root $b$ in $L$. Evaluation at $b$ induces an embedding $E[T]/(h)\to L$, extending the existing embedding to $E(\alpha)$. Repeating for the finitely many roots embeds the constructed [field](../../../../../field.md) $F$ in $L$. They have the same finite cardinality, so this embedding is an [isomorphism](../../../../../isomorphism.md). Thus **the [field](../../../../../field.md) of order $p^s$ is unique up to [isomorphism](../../../../../isomorphism.md)**.

We prove cyclicity of the multiplicative group, also establishing the more general [finite multiplicative subgroup of a field is cyclic](../../../../../finite-multiplicative-subgroup-of-a-field-is-cyclic.md) result. Let $H$ be a finite subgroup of a [field](../../../../../field.md)'s multiplicative group, and let $e$ be the least common multiple of all element orders. For every prime $\ell$ dividing $e$, choose an element whose order has the maximal $\ell$-power $\ell^{a_\ell}$; raising it to the factor of its order coprime to $\ell$ gives an element of order $\ell^{a_\ell}$. Since the group is abelian, the product of these elements has order $\prod_\ell\ell^{a_\ell}=e$: for commuting elements of coprime orders, an equation $(ab)^t=1$ forces $a^t=b^{-t}$ into the intersection of their cyclic subgroups, which is trivial, so both orders divide $t$. Every member of $H$ is a root of $T^e-1$. The [Lagrange root bound over a field](../../../../../lagrange-root-bound-over-a-field.md) gives $|H|\leq e$, while the element just constructed has order $e$ and gives $e\leq|H|$. Thus equality holds and that element generates $H$. In particular

$$
\boxed{\mathbb F_{p^s}^{\times}\cong\mathbb Z/(p^s-1)\mathbb Z.}
$$

For the [field with nine elements](../../../../../field-with-nine-elements.md), use $\mathbb F_3[u]/(u^2+1)$. The [polynomial](../../../../../polynomial-split.md) has no root in $\mathbb F_3$, since its squares are $0,1$, so the quotient is a [field](../../../../../field.md). In the [basis](../../../../../basis.md) $(1,u)$, a vector $(a,b)$ represents $a+bu$, and

$$
(a,b)+(c,d)=(a+c,b+d),\qquad(a,b)(c,d)=(ac-bd,ad+bc)
$$

with coefficients reduced modulo three. Put $\beta=1+u$. Then $\beta^2=2u$, $\beta^4=2=-1$, and $\beta^8=1$, proving that $\beta$ is a [primitive element of a finite field](../../../../../primitive-element-of-a-finite-field.md) of order eight. Its complete power/vector table is

$$
\begin{array}{c|c|c}
\text{label}&\text{element}&\text{vector in }(1,u)\\\hline
a_0&0&(0,0)\\
a_1&\beta^0=1&(1,0)\\
a_2&\beta&(1,1)\\
a_3&\beta^2&(0,2)\\
a_4&\beta^3&(1,2)\\
a_5&\beta^4&(2,0)\\
a_6&\beta^5&(2,2)\\
a_7&\beta^6&(0,1)\\
a_8&\beta^7&(2,1)
\end{array}
$$

For completeness, the full addition and multiplication tables in these labels are displayed below. The subscripts are element labels; they are not the scalar residues of $\mathbb F_3$.

$$
\begin{array}{c|rrrrrrrrr}
+ & a_0 & a_1 & a_2 & a_3 & a_4 & a_5 & a_6 & a_7 & a_8\\\hline
a_0 & a_0 & a_1 & a_2 & a_3 & a_4 & a_5 & a_6 & a_7 & a_8\\
a_1 & a_1 & a_5 & a_8 & a_4 & a_6 & a_0 & a_3 & a_2 & a_7\\
a_2 & a_2 & a_8 & a_6 & a_1 & a_5 & a_7 & a_0 & a_4 & a_3\\
a_3 & a_3 & a_4 & a_1 & a_7 & a_2 & a_6 & a_8 & a_0 & a_5\\
a_4 & a_4 & a_6 & a_5 & a_2 & a_8 & a_3 & a_7 & a_1 & a_0\\
a_5 & a_5 & a_0 & a_7 & a_6 & a_3 & a_1 & a_4 & a_8 & a_2\\
a_6 & a_6 & a_3 & a_0 & a_8 & a_7 & a_4 & a_2 & a_5 & a_1\\
a_7 & a_7 & a_2 & a_4 & a_0 & a_1 & a_8 & a_5 & a_3 & a_6\\
a_8 & a_8 & a_7 & a_3 & a_5 & a_0 & a_2 & a_1 & a_6 & a_4
\end{array}
$$

$$
\begin{array}{c|rrrrrrrrr}
\times & a_0 & a_1 & a_2 & a_3 & a_4 & a_5 & a_6 & a_7 & a_8\\\hline
a_0 & a_0 & a_0 & a_0 & a_0 & a_0 & a_0 & a_0 & a_0 & a_0\\
a_1 & a_0 & a_1 & a_2 & a_3 & a_4 & a_5 & a_6 & a_7 & a_8\\
a_2 & a_0 & a_2 & a_3 & a_4 & a_5 & a_6 & a_7 & a_8 & a_1\\
a_3 & a_0 & a_3 & a_4 & a_5 & a_6 & a_7 & a_8 & a_1 & a_2\\
a_4 & a_0 & a_4 & a_5 & a_6 & a_7 & a_8 & a_1 & a_2 & a_3\\
a_5 & a_0 & a_5 & a_6 & a_7 & a_8 & a_1 & a_2 & a_3 & a_4\\
a_6 & a_0 & a_6 & a_7 & a_8 & a_1 & a_2 & a_3 & a_4 & a_5\\
a_7 & a_0 & a_7 & a_8 & a_1 & a_2 & a_3 & a_4 & a_5 & a_6\\
a_8 & a_0 & a_8 & a_1 & a_2 & a_3 & a_4 & a_5 & a_6 & a_7
\end{array}
$$

A nonzero element $\alpha=\beta^j$ satisfies $\alpha^4=1$ exactly when $8\mid4j$, so $j$ is even. Thus, with $e=1$,

$$
\boxed{\{\alpha:\alpha^4=e\}=\{(1,0),(2,0),(0,1),(0,2)\}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 36](../../paper-36-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
