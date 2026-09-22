<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

There are $(k-1)!$ $k$-cycles in $S_k$, and each has the same [character value of a representation](../../../../../../../character-value-of-a-representation.md) on $S^\lambda$. Taking [traces](../../../../../../../matrix-trace.md) in the [cycle-sum identity for Young–Jucys–Murphy elements](../../../../../../../cycle-sum-identity-for-young-jucys-murphy-elements.md) yields

$$
(k-1)!\,\chi^\lambda(k,1^{n-k})
=\sum_{T\in\operatorname{SYT}(\lambda)}\prod_{r=2}^k c_T(r).
$$

Only tableaux whose first $k$ entries form a [hook partition](../../../../../../../hook-partition.md) contribute.

Write such a shape as $\mu_b=(k-b,1^b)$, for $0\leq b\leq k-1$. There are $f_{\mu_b}=\binom{k-1}{b}$ ways to fill it: choose which $b$ of the labels $2,\ldots,k$ go below the first box. There are $f^{\lambda/\mu_b}$ ways to fill the remaining skew diagram with the labels $k+1,\ldots,n$, in standard order. The [eigenvalue](../../../../../../../eigenvalue.md) from part (ii) is $(-1)^b(k-b-1)!b!$, so the factor

$$
\frac{f_{\mu_b}(k-b-1)!b!}{(k-1)!}
$$

is $1$. Therefore **the general character value is**

$$
\boxed{\chi^\lambda(k,1^{n-k})
=\sum_{\substack{0\leq b\leq k-1\\(k-b,1^b)\subseteq\lambda}}
(-1)^b f^{\lambda/(k-b,1^b)}}.
$$

Here $f^{\lambda/\mu}$ counts [standard skew Young tableaux](../../../../../../../standard-skew-young-tableau.md), and is zero when $\mu$ is not contained in $\lambda$. In particular, for a full $n$-cycle,

$$
\boxed{
\chi^\lambda(n)=
\begin{cases}
(-1)^b,&\lambda=(n-b,1^b),\\
0,&\lambda\text{ is not a hook}.
\end{cases}}
$$

For $k=1$, the general formula gives $f^{\lambda/(1)}=f_\lambda$, the character value at the identity, as it should.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
