<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

In a commutative [ring](../../../../../ring.md), if $x^m=0$, then the principal [ideal](../../../../../ideal.md) $(x)$ satisfies $(x)^m=0$. Thus a [semiprime ring](../../../../../semiprime-ring.md) has no nonzero [nilpotent elements](../../../../../nilpotent.md). Conversely, if $I^m=0$ for an [ideal](../../../../../ideal.md) $I$, then every $x\in I$ satisfies $x^m=0$; absence of nonzero [nilpotent elements](../../../../../nilpotent.md) forces $I=0$. Hence **commutative semiprimeness is exactly reducedness**.

For a [prime ideal](../../../../../prime-ideal.md) $P$, let $S=R\setminus P$. Every [ideal](../../../../../ideal.md) $I$ of $R_P=S^{-1}R$ is the extension of its contraction $I^c$: if $r/s\in I$, multiply by the [unit](../../../../../unit-in-a-ring.md) $s/1$ to get $r/1\in I$, so $r\in I^c$. If $R$ is [Noetherian](../../../../../noetherian-ring.md), write $I^c=(r_1,\ldots,r_m)$; their images generate $I$. This proves that $R_P$ is [Noetherian](../../../../../noetherian-ring.md).

The extended [ideal](../../../../../ideal.md) $PR_P$ is proper. Indeed $1=p/s$ would imply $u(s-p)=0$ for some $u\notin P$, and then $us=up\in P$, contradicting primeness and $u,s\notin P$. A fraction with numerator outside $P$ is invertible, with inverse $s/r$. A fraction with numerator in $P$ lies in the proper [ideal](../../../../../ideal.md) $PR_P$ and cannot be invertible. Thus the nonunits are precisely $PR_P$, making it the unique maximal [ideal](../../../../../ideal.md). Therefore

$$
\boxed{R_P\text{ is a Noetherian local ring with maximal ideal }PR_P.}
$$

To prove reducedness is detected by prime localizations, let $x$ be a [nilpotent element](../../../../../nilpotent.md) of $R$. Its image in every $R_Q$ is zero because these localizations are semiprime, hence reduced. If $x\ne0$, its [annihilator](../../../../../annihilator-ring-theory.md) $\operatorname{Ann}(x)$ is a proper [ideal](../../../../../ideal.md); choose a maximal [ideal](../../../../../ideal.md) $Q$ containing it. The zero criterion for [localization](../../../../../localization-of-a-ring.md) says $x/1=0$ in $R_Q$ only if $sx=0$ for some $s\notin Q$, which would put $s$ in $\operatorname{Ann}(x)\subseteq Q$, a contradiction. Hence $x=0$, and $R$ is semiprime. This argument does not need Noetherianity.

Primeness is not detected in the same way. Take **$R=k\times k$**. Its two [prime ideals](../../../../../prime-ideal.md) are $P_1=0\times k$ and $P_2=k\times0$, and its corresponding localizations are both isomorphic to the [field](../../../../../field.md) $k$. To see these are all the [prime ideals](../../../../../prime-ideal.md), the orthogonal [idempotents](../../../../../idempotent.md) $e_1,e_2$ have product zero, so a [prime ideal](../../../../../prime-ideal.md) contains one of them and is then the kernel of the other projection. Both localizations are prime [rings](../../../../../ring.md), but $R$ is not prime: $e_1,e_2\ne0$ and $e_1e_2=0$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 85](../../paper-85-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
