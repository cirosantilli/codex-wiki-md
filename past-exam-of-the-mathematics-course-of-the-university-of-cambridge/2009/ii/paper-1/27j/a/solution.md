<h1 id="27j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the natural [filtration](../../../../../../filtration-probability-theory.md) $\mathcal F_t=\sigma(X_s:s\leq t)$, a [stopping time](../../../../../../stopping-time.md) $T$ takes values in $[0,\infty]$ and satisfies $\{T\leq t\}\in\mathcal F_t$ for every $t$. Its occurrence is decidable from information available by that time.

The [Strong Markov property](../../../../../../strong-markov-property.md) says that on $T<\infty$, conditionally on $X_T$, the post-$T$ process is independent of $\mathcal F_T$ and has the law of the original [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md) started at $X_T$. In particular $\mathbb E_i[f(X_{T+s})\mid\mathcal F_T]=P_sf(X_T)$ on $T<\infty$. The chain is an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md) if every state communicates with every other: for any $i,j$ some time has $\mathbb P_i(X_t=j)>0$, equivalently for finite rates there is a path of positive off-diagonal jump rates between them.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [27J](../../27j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
