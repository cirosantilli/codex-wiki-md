<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $T_3(A)$ count ordered solutions $a+c=2b$ in $A^3$, including the trivial ones. The hypothesis gives $T_3(A)\ge cn^2$. Its relation to [additive energy](../../../../../../additive-energy.md) is the promised easy Fourier step. Translate $A$ into $[0,M]$ and embed it in an odd prime cyclic group of order $P>4M$. No relevant integer equality wraps modulo $P$. With the unnormalized [Fourier transform](../../../../../../fourier-transform.md) $\widehat f(r)=\sum_x1_A(x)e(-rx/P)$, [character orthogonality](../../../../../../character-orthogonality.md) gives

$$
T_3(A)=\frac1P\sum_r\widehat f(r)^2\widehat f(-2r),\qquad
E(A)=\frac1P\sum_r|\widehat f(r)|^4.
$$

Since multiplication by $2$ permutes the characters, [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) and [Parseval identity on a finite group](../../../../../../parseval-identity-on-a-finite-group.md) imply

$$
T_3(A)^2\le E(A)\left(\frac1P\sum_r|\widehat f(-2r)|^2\right)=nE(A).
$$

Thus $E(A)\ge c^2n^3$. Equivalently, one can apply [Cauchy-Schwarz](../../../../../../cauchy-schwarz-inequality.md) directly to $T_3(A)=\sum_{b\in A}r_{A+A}(2b)$.

By part (i), some $B\subseteq A$ has $|B|\ge c_1(c)n$ and $|B+B|\le K(c)|B|$. Part 3(ii) then bounds $|2B-2B|\le K(c)^4|B|$. Apply part (ii) with $k=2$: there is $B'\subseteq B$, $|B'|\ge|B|/3$, [Freiman 2-isomorphic](../../../../../../freiman-2-isomorphism.md) to a subset $C\subseteq\mathbb Z_N$ with $N\le4K(c)^4|B|+1$. Consequently $C$ has a positive [subset density](../../../../../../density-of-a-finite-subset.md) depending only on $c$, and $N$ tends to infinity with $n$ because $N\ge|B'|$.

View the representatives of $C$ as a subset of $\{0,\ldots,N-1\}$. The assumed four-term case of [Szemerédi's theorem](../../../../../../szemeredi-s-theorem.md) gives four distinct integer representatives in arithmetic progression once $n$ is sufficiently large in terms of $c$. If their preimages are $b_0,b_1,b_2,b_3$, the two model equalities

$$
\theta(b_0)+\theta(b_2)=2\theta(b_1),\qquad
\theta(b_1)+\theta(b_3)=2\theta(b_2)
$$

lift through the [Freiman 2-isomorphism](../../../../../../freiman-2-isomorphism.md) to the same equalities in $\mathbb Z$. Hence their consecutive differences agree; injectivity makes the common difference nonzero. Therefore **$A$ contains a nonconstant four-term arithmetic progression**. This proves [dense three-term progressions force four-term progressions](../../../../../../dense-three-term-progressions-force-four-term-progressions.md) without an assumption that $A$ initially lies in a short interval.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
