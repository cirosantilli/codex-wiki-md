<h1 id="20h/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each rational prime $p$, define

$$
\chi(p)=
\begin{cases}
1,&(p)=\mathfrak p_1\mathfrak p_2\text{ with }\mathfrak p_1\ne\mathfrak p_2,\\
-1,&(p)\text{ remains prime in }\mathcal O_K,\\
0,&(p)=\mathfrak p^2\text{ is ramified}.
\end{cases}
$$

These are the three cases in [splitting of rational primes in a quadratic field](../../../../../../../splitting-of-rational-primes-in-a-quadratic-field.md).

Set $x=p^{-s}$. In the split case the local factor of the [Dedekind zeta function](../../../../../../../dedekind-zeta-function.md) is $(1-x)^{-2}$; in the inert case it is $(1-x^2)^{-1}$ because the prime ideal has norm $p^2$; and in the ramified case it is $(1-x)^{-1}$. On the other hand, the product of the local factors of $\zeta_{\mathbb Q}(s)$ and $L(\chi,s)$ is

$$
(1-x)^{-1}(1-\chi(p)x)^{-1},
$$

which gives exactly those three expressions when $\chi(p)=1,-1,0$. Multiplying over all rational primes proves the [quadratic Dedekind zeta factorization](../../../../../../../quadratic-dedekind-zeta-factorization.md)

$$
\zeta_K(s)=\zeta_{\mathbb Q}(s)L(\chi,s)
$$

formally.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [20H](../../../20h.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
