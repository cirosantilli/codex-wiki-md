<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

It suffices first to treat [unital algebras](../../../../../../unital-algebra.md) and a [unital](../../../../../../unital-algebra.md) [homomorphism](../../../../../../homomorphism.md). A surjective [homomorphism](../../../../../../homomorphism.md) between [unital algebras](../../../../../../unital-algebra.md) automatically preserves the identity. If $B=0$, [continuity](../../../../../../continuous-function.md) is immediate. In the nonunital case, extend to the forced [unitizations](../../../../../../unitization-of-an-algebra.md) by $T^+(a+\lambda1)=T(a)+\lambda1$. This is still surjective and the [unitization](../../../../../../unitization-of-an-algebra.md) of a semisimple algebra is semisimple: its radical projects to zero in its scalar quotient, and its remaining intersection with the original algebra is its original radical. [Continuity](../../../../../../continuous-function.md) of the extension implies [continuity](../../../../../../continuous-function.md) of the original map.

An [algebra homomorphism](../../../../../../algebra-homomorphism-over-a-field.md) decreases the [spectral radius](../../../../../../spectral-radius.md), even without any [continuity](../../../../../../continuous-function.md) assumption, because it takes an inverse of $\lambda1-a$ to an inverse of $\lambda1-T(a)$. Suppose $a_n\to0$ in $A$ and $T(a_n)\to b$ in $B$. Fix any $c\in B$ and choose $u,v\in A$ with $T(u)=b$, $T(v)=c$. Put

$$
w=vu,\quad w_n=va_n,\quad d=T(w)=cb,\quad d_n=T(w_n)\longrightarrow d.
$$

Consider the [polynomial](../../../../../../polynomial-split.md) $q_n(z)=T((1-z)w_n+zw)=(1-z)d_n+zd$. Its value at one is exactly $d$. On the outer circle $|z|=R$,

$$
r_B(q_n(z))\le\|q_n(z)\|\le\|d\|+(1+R)\|d_n-d\|.
$$

On the inner circle $|z|=1/R$, spectral-radius decrease gives

$$
r_B(q_n(z))\le r_A((1-z)w_n+zw)
\le(1+1/R)\|w_n\|+\|w\|/R.
$$

Applying part (i) in $B$ and then letting $n\to\infty$, with $R$ fixed, gives

$$
r_B(cb)^2\le\frac{\|cb\|\|vu\|}{R}.
$$

This holds for every $R>1$, so **$r_B(cb)=0$ for every $c\in B$**.

This forces $b$ into the [Jacobson radical](../../../../../../jacobson-radical.md). To see the criterion directly, if $b$ were outside a [maximal left ideal](../../../../../../maximal-left-ideal.md) $L$, then $L+Bb=B$, so $1=l+cb$ for some $l\in L$, $c\in B$. The equality $r_B(cb)=0$ makes $1-cb$ invertible, but this element equals $l\in L$, impossible in a proper [left ideal](../../../../../../left-ideal.md). Hence $b$ lies in every [maximal left ideal](../../../../../../maximal-left-ideal.md). Since $B$ is semisimple, $b=0$.

We have shown that the separating space of $T$ is zero. If $a_n\to a$ and $T(a_n)\to y$, apply the result to $a_n-a$ to obtain $y=T(a)$. Its graph is [closed](../../../../../../closed-set.md), and the [closed graph theorem](../../../../../../closed-graph-theorem.md) now proves

$$
\boxed{T\text{ is continuous}.}
$$

The crucial estimate uses part (i) with an exactly fixed central value; it does not assume the false general assertion that the [spectral radius](../../../../../../spectral-radius.md) is [continuous](../../../../../../continuous-function.md) under [norm](../../../../../../norm.md) limits.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
