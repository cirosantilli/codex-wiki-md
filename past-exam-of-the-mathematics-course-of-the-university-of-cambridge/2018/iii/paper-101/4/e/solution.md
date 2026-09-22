<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**No.** Take $R=k[t]$ over a [field](../../../../../../field.md) $k$, and inside $R[x]=k[t,x]$ take

$$
S=k[t]+tx\,k[t,x].
$$

This is a subring containing $R$: its elements have arbitrary constant coefficient in $k[t]$ as polynomials in $x$, and every positive-degree coefficient is divisible by $t$; that condition is preserved by sums and products. The [ring](../../../../../../ring.md) $R$ is [Noetherian](../../../../../../noetherian-ring.md). Indeed, a nonzero [ideal](../../../../../../ideal.md) of $k[t]$ has an element $g$ of least degree, and division by $g$ shows that every element of the [ideal](../../../../../../ideal.md) is a multiple of $g$. Thus $k[t]$ is a [principal ideal domain](../../../../../../principal-ideal-domain.md), and its [ideals](../../../../../../ideal.md) are finitely generated.

In $S$, let $J_n=(tx,tx^2,\ldots,tx^n)_S$. These form an ascending chain. We show that $tx^{n+1}\notin J_n$. If it belonged, we could write

$$
tx^{n+1}=\sum_{j=1}^n s_jtx^j,\qquad s_j\in S.
$$

Cancel $t$ in the [integral domain](../../../../../../integral-domain.md) $k[t,x]$, then apply the [evaluation homomorphism](../../../../../../evaluation-homomorphism.md) $t\mapsto0$. Every $s_j\in S$ becomes a scalar in $k$, so this would give

$$
x^{n+1}=\sum_{j=1}^n s_j(0,x)x^j,\qquad s_j(0,x)\in k,
$$

which is impossible by comparison of degrees. Hence $J_n\subsetneq J_{n+1}$ for every $n$, and

$$
\boxed{k[t]\subseteq k[t]+txk[t,x]\subseteq k[t,x],\quad
k[t]\text{ Noetherian but }k[t]+txk[t,x]\text{ not Noetherian}.}
$$

This is a [constant-plus-ideal non-Noetherian subring](../../../../../../constant-plus-ideal-non-noetherian-subring.md) construction: the restricted coefficients prevent a finite list of positive powers of $x$ from generating all the required powers.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
