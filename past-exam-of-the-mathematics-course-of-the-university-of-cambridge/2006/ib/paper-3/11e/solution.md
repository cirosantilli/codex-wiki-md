<h1 id="11e/solution">Solution</h1>

↑ **Parent:** [11E](../11e.md)

Use the usual commutative unital-ring convention for [Noetherian rings](../../../../../noetherian-ring.md). A ring is Noetherian exactly when every [ideal](../../../../../ideal.md) is finitely generated, equivalently when ascending chains of [ideals](../../../../../ideal.md) stabilize. Indeed, the union of an ascending chain is an [ideal](../../../../../ideal.md); finitely many generators all lie in a single chain member. Conversely, if an [ideal](../../../../../ideal.md) cannot be finitely generated, adjoining a new element at each stage constructs a strictly ascending chain.

First assume $R[X]$ is Noetherian. Evaluation at zero gives a surjective [ring homomorphism](../../../../../ring-homomorphism.md) $R[X]\to R$ with [kernel](../../../../../kernel-of-a-linear-map.md) $(X)$. A quotient of a [Noetherian ring](../../../../../noetherian-ring.md) is Noetherian: lift an [ideal](../../../../../ideal.md) to the source, take finitely many generators there, and map those generators down. Thus $R\cong R[X]/(X)$ is Noetherian.

For the converse, assume $R$ is Noetherian and take any [ideal](../../../../../ideal.md) $I\subseteq R[X]$. For $d\ge0$, let $J_d$ be the set of coefficients of $X^d$ in elements of $I$ of degree at most $d$. It is an [ideal](../../../../../ideal.md) of $R$, since sums and scalar multiples of such [polynomials](../../../../../polynomial-split.md) stay in $I$. Multiplication by $X$ shows $J_d\subseteq J_{d+1}$. The ascending chain stabilizes, say at $N$.

For each $0\le d\le N$, choose finitely many generators $a_{d,j}$ of $J_d$ and corresponding $f_{d,j}\in I$ of degree at most $d$ having coefficient $a_{d,j}$ at $X^d$. Discard zero generators. We claim these finitely many [polynomials](../../../../../polynomial-split.md) generate $I$. If a nonzero $f\in I$ has degree $m\le N$, express its leading coefficient as $\sum_jr_j a_{m,j}$ and subtract $\sum_jr_jf_{m,j}$. The degree decreases. If $m>N$, use $J_m=J_N$, express the leading coefficient using the $a_{N,j}$, and subtract

$$
\sum_jr_jX^{m-N}f_{N,j}.
$$

Again the leading term cancels and the degree decreases. Induction on degree, including degree zero, expresses every $f$ in the claimed [ideal](../../../../../ideal.md). Therefore every [ideal](../../../../../ideal.md) of $R[X]$ is finitely generated, proving the [Hilbert basis theorem](../../../../../hilbert-basis-theorem.md) and

$$
\boxed{R[X]\text{ is Noetherian}\iff R\text{ is Noetherian}.}
$$

The argument is the [bounded-degree coefficient proof of Hilbert basis theorem](../../../../../bounded-degree-coefficient-proof-of-hilbert-basis-theorem.md); it never divides by a leading coefficient and therefore does not require $R$ to be an [integral domain](../../../../../integral-domain.md). With the analogous left-ideal convention the same proof applies to left-Noetherian rings with a central indeterminate.

## ↑ Ancestors (10)

1. [11E](../11e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
