<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the allowed reduction $[N,G,G,G]=1$. Set $C=[N,G]$ and $D=[C,G]$. Then $[D,G]=1$, so $D$ is central. For $n\in N$ and $g\in G$, put $c=[n,g]$. The identity $[ab,g]=[a,g]^b[b,g]$ and centrality of $[c,n]\in D$ give, by induction on $k$,

$$
[n^k,g]=c^k[c,n]^{\binom{k}{2}}.
$$

At $k=p$, both factors belong to $C^p$: the first is a $p$th power in $C$, and the second is a $p$th power because $p\mid\binom p2$ and $[c,n]\in D\leq C$. The [subgroup](../../../../../../subgroup.md) $C^p$ is normal in $G$. Commuting products of the generators $n^p$ with $g$ and using the same identity consequently yields

$$
[N^p,G]\leq C^p.
$$

Since $C=[N,G]\leq N^p$, it follows that $[C,G]\leq C^p$. **Thus $[N,G]$ is powerfully embedded.** This proves the reduced case, and the reduction permitted in the question gives the general assertion.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
