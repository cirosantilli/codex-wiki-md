<h1 id="11e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Induct on $n$ to prove the stronger assertion that any [submodule](../../../../../../submodule.md) $M\subseteq R^n$ is a [free module](../../../../../../free-module.md) of [rank of a free module](../../../../../../rank-of-a-free-module.md) at most $n$. For $n=0$ this is immediate. Project onto the first coordinate by $\pi:R^n\to R$. Its image $\pi(M)$ is an [ideal](../../../../../../ideal.md) of the [principal ideal domain](../../../../../../principal-ideal-domain.md), so $\pi(M)=(a)$.

If $a=0$, then $M$ embeds in the remaining $n-1$ coordinates and the induction hypothesis applies. Otherwise choose $v\in M$ with $\pi(v)=a$. Put $N=M\cap\ker\pi$, a [submodule](../../../../../../submodule.md) of $R^{n-1}$, which is free by induction. For every $m\in M$, there is $b\in R$ with $\pi(m)=ba$, so $m-bv\in N$. If $bv\in N$, then $ba=0$; the [integral domain](../../../../../../integral-domain.md) property and $a\ne0$ give $b=0$. Therefore

$$
\boxed{M=Rv\oplus N\cong R\oplus N}.
$$

Appending $v$ to a [basis](../../../../../../basis.md) of $N$ proves that $M$ is a [free module](../../../../../../free-module.md) of [rank of a free module](../../../../../../rank-of-a-free-module.md) at most $n$. This proof of the [submodule theorem for free modules over a principal ideal domain](../../../../../../submodule-theorem-for-free-modules-over-a-principal-ideal-domain.md) does not assume in advance that $M$ is a [finitely generated module](../../../../../../finitely-generated-module.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
