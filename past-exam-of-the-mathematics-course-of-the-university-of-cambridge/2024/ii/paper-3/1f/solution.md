<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

Write $N=\prod_i p_i^{e_i}$ with odd primes $p_i$. The [Jacobi symbol](../../../../../jacobi-symbol.md) is

$$
\left(\frac aN\right)=\prod_i\left(\frac a{p_i}\right)^{e_i},
$$

where each factor on the right is a Legendre symbol. The supplementary law is

$$
\left(\frac2N\right)=(-1)^{(N^2-1)/8}.
$$

For coprime positive odd $m,n$, [quadratic reciprocity](../../../../../quadratic-reciprocity.md) gives

$$
\left(\frac mn\right)\left(\frac nm\right)
=(-1)^{(m-1)(n-1)/4}.
$$

Applying this with $m=3$ gives

$$
\left(\frac3N\right)=
\begin{cases}
 1,&N\equiv1,11\pmod {12},\\
-1,&N\equiv5,7\pmod {12},\\
 0,&3\mid N.
\end{cases}
$$

Finally, factor $d=2^e m$ with $m$ odd. The supplementary laws for $-1$ and $2$, followed by reciprocity on every odd prime factor of $m$, express $(-d/a)$ solely in terms of the residue class of the positive odd integer $a$ modulo $d$ when $d\equiv0$ or $3\pmod4$. If $a\equiv b\pmod d$, all those factors, including the zero cases, agree; hence

$$
\boxed{\left(\frac{-d}{a}\right)=\left(\frac{-d}{b}\right).}
$$

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
