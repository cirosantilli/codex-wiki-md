<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The equivalence is **true**. Write $c_r(\eta)$ for the total size at level $r$ of the [core tower of a partition](../../../../../../core-tower-of-a-partition.md) $\eta$, and $q_r(\eta)$ for the corresponding total size in its [quotient tower of a partition](../../../../../../quotient-tower-of-a-partition.md). We use the size relation and the [P-adic valuation of a symmetric-group character degree from the core tower](../../../../../../p-adic-valuation-of-a-symmetric-group-character-degree-from-the-core-tower.md):

$$
|\eta|=\sum_{r\geq0}c_r(\eta)p^r,
\qquad
\nu_p(\chi^\eta(1))=\frac{\sum_{r\geq0}c_r(\eta)-d_p(|\eta|)}{p-1}.
$$

Here $d_p$ is the [base-p digit sum](../../../../../../base-p-digit-sum.md). These imply the [character degree coprime to p from the core tower](../../../../../../character-degree-coprime-to-p-from-the-core-tower.md) criterion: if $|\eta|=\sum_r\alpha_rp^r$, then $p\nmid\chi^\eta(1)$ exactly when $c_r(\eta)=\alpha_r$ at every level. Indeed carrying $p$ units from one position to the next decreases the sum of coefficients by $p-1$; the valuation vanishes precisely when there are no carries.

For $k\geq1$, we also use [power-core truncation of a prime-core tower](../../../../../../power-core-truncation-of-a-prime-core-tower.md): for $\gamma=C_{p^k}(\lambda)$, its core tower agrees with that of $\lambda$ below level $k$ and is empty at every level at least $k$. Moreover $q_k(\lambda)=w_{p^k}(\lambda)$, the [weight of a partition](../../../../../../weight-of-a-partition.md) for modulus $p^k$. To see the truncation, removal of a [rim hook](../../../../../../rim-hook.md) of length $p^k$ preserves the first $p$-core and, under the [abacus divisible-hook correspondence](../../../../../../hooks-divisible-by-the-abacus-modulus.md), becomes removal of a $p^{k-1}$-hook in one quotient component. Iterating preserves all the lower cores; after all such removals, quotient level $k$ is empty.

If $p\nmid\chi^\lambda(1)$, the criterion gives $c_k(\lambda)=a$, $c_r(\lambda)=0$ for $r>k$, and the lower $c_r(\lambda)$ are the base-$p$ digits of $m$. It follows that $|\gamma|=m$, $p\nmid\chi^\gamma(1)$ and

$$
w_{p^k}(\lambda)=\frac{n-|\gamma|}{p^k}=a.
$$

Conversely, suppose $w_{p^k}(\lambda)=a$ and $p\nmid\chi^\gamma(1)$. Then $|\gamma|=m$ and its lower core-tower sizes are the digits of $m$. Quotient level $k$ of $\lambda$ has total size $a<p$. Each component there has size less than $p$, hence is already a $p$-core and has empty $p$-quotient. Thus $c_k(\lambda)=a$ and every higher level is empty. Combined with truncation, this gives exactly the digits of $n$, so $p\nmid\chi^\lambda(1)$.

Therefore

$$
\boxed{p\nmid\chi^\lambda(1)\ \Longleftrightarrow\ w_{p^k}(\lambda)=a\text{ and }p\nmid\chi^{C_{p^k}(\lambda)}(1).}
$$

If $k=0$, necessarily $m=0$ and $n=a<p$; the $1$-core is empty, its weight is $n=a$, and the [Hook-length formula](../../../../../../hook-length-formula.md) shows that every degree is coprime to $p$. Thus the equivalence holds in that boundary case too, with the empty partition having degree one.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
