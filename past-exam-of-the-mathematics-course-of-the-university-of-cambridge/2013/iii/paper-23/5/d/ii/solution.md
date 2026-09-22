<h1 id="5/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the progression [integers](../../../../../../../integer.md) as $n=a+qm$. Their $m$ values lie in an interval of length at most $N/q+1$. For every [prime](../../../../../../../prime-number.md) $p\nmid q$, primality forbids the unique residue $m\equiv-aq^{-1}\pmod p$; [primes](../../../../../../../prime-number.md) dividing $q$ impose no restriction because $(a,q)=1$.

Choose $Q=\max(2,\lfloor\sqrt{N/q}\rfloor)$. The selected [primes](../../../../../../../prime-number.md) exceed $M>N$, hence exceed these sieving [primes](../../../../../../../prime-number.md). The uniform coprime-denominator estimate just proved yields

$$
|S|\ll\frac{N/q+Q^2+1}{(\varphi(q)/q)\log(2Q)}
\ll\frac{N}{\varphi(q)\log(N/q)}.
$$

The assumption $N\ge q^{2+\delta}$ implies $\log(N/q)\ge\frac{1+\delta}{2+\delta}\log N\ge\frac12\log N$. Therefore

$$
\boxed{\pi(M+N;q,a)-\pi(M;q,a)\ll\frac{N}{\varphi(q)\log N}.}
$$

Endpoint and bounded small-parameter corrections are again absorbed. The proof supplies the more informative short-interval progression bound before using the given size hypothesis.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Paper 23](../../../../paper-23-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
