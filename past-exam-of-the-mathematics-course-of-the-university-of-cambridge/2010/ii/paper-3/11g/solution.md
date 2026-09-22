<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

The [Miller-Rabin primality test](../../../../../miller-rabin-primality-test.md) first handles $2,3$ as [prime](../../../../../prime-number.md) and $n<2$ or even $n>2$ as composite. For odd $n>3$, write $n-1=2^s d$ with $d$ odd and choose a base $2\le a\le n-2$. A nontrivial $\gcd(a,n)$ proves compositeness. Otherwise compute $x=a^d\bmod n$: the round passes if $x=1$ or $x=-1$. If neither holds, square successively, at most $s-1$ times, and pass if a value $-1$ occurs; otherwise declare composite. An occurrence of $1$ before $-1$ exhibits a nontrivial square root of one and is also a failure. For [prime](../../../../../prime-number.md) $n$, Fermat's theorem and the fact that a field has only the square roots $\pm1$ force a pass. The standard strong-liar bound says that an odd composite passes for at most one quarter of the bases; independent random rounds therefore have error probability at most $4^{-r}$ after $r$ rounds. Passing is a probable-prime verdict, not a proof of primality. A [Fermat pseudoprime](../../../../../fermat-pseudoprime.md) is composite and passes $a^{n-1}\equiv1\pmod n$; a [strong pseudoprime](../../../../../strong-pseudoprime.md) is composite and passes the stronger round above.

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
