<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Let $M=\{i:x\in A_i\}$, with $|M|=m$. Then $\mathbf1_{A_S}(x)=1$ exactly when $S\subseteq M$, and the sum becomes

$$
\sum_{s=t}^{m}\binom ms\binom st(-1)^{s-t}
=\binom mt\sum_{r=0}^{m-t}\binom{m-t}{r}(-1)^r
=\binom mt(1-1)^{m-t}.
$$

This is $1$ when $m=t$ and $0$ otherwise. Summing over $x\in X$ yields

$$
\boxed{\#\{x:x\text{ belongs to exactly }t\text{ sets}\}
=\sum_S\binom{|S|}{t}(-1)^{|S|-t}|A_S|.}
$$

Taking the complement of the $t=0$ case gives the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md)

$$
\left|\bigcup_iA_i\right|=\sum_{\varnothing\ne S}(-1)^{|S|+1}|A_S|.
$$

If $p_1,\ldots,p_r$ are the distinct prime divisors of $N$, inclusion-exclusion removes their multiples from $\{1,\ldots,N\}$ and gives

$$
\boxed{\varphi(N)=N\prod_{p\mid N}\left(1-\frac1p\right).}
$$

For the stated squarefree $n=q_1\cdots q_k$ and $\gcd(x,n)=1$, Fermat's theorem gives $x^{q_j-1}\equiv1\pmod{q_j}$. Since $q_j-1\mid n-1$, every $q_j$ divides $x^{n-1}-1$; their product does too. Thus **$n$ is a Carmichael number**.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
