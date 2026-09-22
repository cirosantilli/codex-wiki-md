<h1 id="20g/solution">Solution</h1>

↑ **Parent:** [20G](../20g.md)

The factorization form of [Kummer-Dedekind theorem](../../../../../kummer-dedekind-theorem.md) is as follows. If $K=\mathbb Q(\theta)$ with $\theta$ integral, minimal [polynomial](../../../../../polynomial-split.md) $f$, and $p$ does not divide the index $[\mathcal O_K:\mathbb Z[\theta]]$, factor $\bar f=\prod_i\bar f_i^{e_i}$ into distinct monic [irreducibles](../../../../../irreducible-representation.md) over $\mathbb F_p$. Then

$$
p\mathcal O_K=\prod_i\mathfrak p_i^{e_i},\qquad
\mathfrak p_i=(p,f_i(\theta)),\qquad
[\mathcal O_K/\mathfrak p_i:\mathbb F_p]=\deg f_i.
$$

The index condition is essential. All integral bases used below make the index one, so it applies to every [prime](../../../../../prime-number.md).

For a [squarefree](../../../../../squarefree-integer.md) quadratic $d\equiv2,3\pmod4$, take $\theta=\sqrt d$, $f=X^2-d$ and field [discriminant](../../../../../discriminant.md) $D=4d$. At an odd [prime](../../../../../prime-number.md), a repeated factor occurs exactly when $p\mid d$, in which case $\bar f=X^2$ and $p\mathcal O_K=(p,\sqrt d)^2$. At $p=2$, reduction is $X^2$ if $d$ is even and $(X+1)^2$ if $d$ is odd, so $2$ is totally ramified in both cases. Thus the totally ramified [primes](../../../../../prime-number.md) are exactly those dividing $4d$.

For $d\equiv1\pmod4$, take $\theta=(1+\sqrt d)/2$, with [polynomial](../../../../../polynomial-split.md) $X^2-X+(1-d)/4$ and [discriminant](../../../../../discriminant.md) $D=d$. At an odd [prime](../../../../../prime-number.md) it has a double root exactly when $p\mid d$, giving a single linear factor squared and total ramification. At $p=2$, its [derivative](../../../../../derivative.md) is $1$, so no repeated factor occurs. Hence again

$$
\boxed{p\text{ is totally ramified }\Longleftrightarrow p\mid D}.
$$

For the [prime](../../../../../prime-number.md) [cyclotomic field](../../../../../cyclotomic-field.md), use $\Phi_q(X)=1+X+\cdots+X^{q-1}$. Modulo $q$ this is $(X-1)^{q-1}$, so $q\mathcal O_K=(q,\zeta-1)^{q-1}$, proving total ramification. For $p\ne q$, the [discriminant](../../../../../discriminant.md) has no [prime](../../../../../prime-number.md) factor $p$, so the reduction is [squarefree](../../../../../squarefree-integer.md) and $p$ is unramified. There is an actual exponent error in the printed [discriminant](../../../../../discriminant.md): the correct value is $(-1)^{(q-1)/2}q^{q-2}$, not $q^{q-1}$. To check it, at a nontrivial root $\zeta^j$,

$$
\Phi_q'(\zeta^j)=\frac{q(\zeta^j)^{q-1}}{\zeta^j-1},
$$

and multiplying these [derivatives](../../../../../derivative.md) and using $\prod_{j=1}^{q-1}(1-\zeta^j)=q$ gives the exponent $q-2$. The [prime](../../../../../prime-number.md) support is still just $\{q\}$, so the requested ramification conclusion is unaffected.

For $\theta=\sqrt[3]2$, the [integral basis](../../../../../integral-basis.md) gives $f=X^3-2$ and $D=-108$. Modulo $2$, $\bar f=X^3$; modulo $3$, $\bar f=(X+1)^3$. Dedekind factorization gives $(2)=(2,\theta)^3$ and $(3)=(3,\theta+1)^3$. For other [primes](../../../../../prime-number.md) the [polynomial](../../../../../polynomial-split.md) is [squarefree](../../../../../squarefree-integer.md) because its [discriminant](../../../../../discriminant.md) is not divisible by the [prime](../../../../../prime-number.md). Therefore the equivalence also holds in this cubic field. This is a conclusion for these specific fields, not the false general assertion that every ramified [prime](../../../../../prime-number.md) in every higher-degree number field is totally ramified.

## ↑ Ancestors (10)

1. [20G](../20g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
