<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

The [Möbius function](../../../../../mobius-function.md) is defined by $\mu(1)=1$ and, for $n>1$,

$$
\mu(n)=
\begin{cases}
0,&p^2\mid n\text{ for some prime }p,\\
(-1)^r,&n\text{ is a product of }r\text{ distinct primes}.
\end{cases}
$$

It is a [multiplicative arithmetic function](../../../../../multiplicative-function.md): $\mu(mn)=\mu(m)\mu(n)$ whenever $m$ and $n$ are [coprime](../../../../../coprime-integers.md).

The summand $\mu(d)^2/\phi(d)$ is multiplicative, so its [divisor sum](../../../../../divisor-sum.md) is multiplicative. For a [prime power](../../../../../prime-power.md) $p^a$ with $a\geq1$, only $d=1,p$ contribute and

$$
\sum_{d\mid p^a}\frac{\mu(d)^2}{\phi(d)}
=1+\frac1{p-1}=\frac p{p-1}
=\frac{p^a}{\phi(p^a)}.
$$

Multiplying these local identities over the prime divisors of $n$ gives

$$
\boxed{\sum_{d\mid n}\frac{\mu(d)^2}{\phi(d)}=\frac n{\phi(n)}}.
$$

For the final claim, choose distinct primes $p_0,\ldots,p_k$. The moduli $p_j^2$ are pairwise coprime, so the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) gives an integer $a$ satisfying

$$
a\equiv-j\pmod{p_j^2},\qquad 0\leq j\leq k.
$$

Every positive integer $n\equiv a\pmod{\prod_jp_j^2}$ then has $p_j^2\mid n+j$. Hence

$$
\boxed{\mu(n)=\mu(n+1)=\cdots=\mu(n+k)=0}.
$$

There are infinitely many positive representatives of this congruence class.

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
