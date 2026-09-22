<h1 id="17h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $k\geq1$ and sample $G$ from the [Erdős-Rényi model](../../../../../../erdos-renyi-model.md) with $p=\tfrac12n^{-2/3}$. Let $X$ count copies of the [complete bipartite graph](../../../../../../complete-bipartite-graph.md) $K_{3,3}$. By the [expected subgraph count in the Erdős-Rényi model](../../../../../../expected-subgraph-count-in-the-erdos-renyi-model.md),

$$
\mathbb EX
=\frac12\binom n3\binom{n-3}3p^9
\longrightarrow \frac{1}{72\,2^9}<1.
$$

Put $m=\lceil n/k\rceil$ and let $Z$ count [independent set](../../../../../../independent-set-graph-theory.md) of size $m$. If the [chromatic number](../../../../../../chromatic-number.md) satisfies $\chi(G)\leq k$, some colour class has at least $m$ vertices, so $Z\geq1$. Moreover,

$$
\begin{aligned}
\mathbb EZ
&=\binom nm(1-p)^{\binom m2}\\
&\leq\left(\frac{en}{m}\right)^m
   \exp\left(-p\binom m2\right)
\longrightarrow0,
\end{aligned}
$$

because the positive part of the exponent is $O(n)$ whereas $p\binom m2$ has order $n^{4/3}$. The [first moment method](../../../../../../first-moment-method.md) therefore gives $\mathbb P(\chi(G)\leq k)\leq\mathbb EZ=o(1)$.

Using [Markov inequality](../../../../../../markov-inequality.md) for $X$ and the [union bound](../../../../../../boole-s-inequality.md),

$$
\begin{aligned}
\mathbb P(X=0\text{ and }\chi(G)>k)
&\geq1-\mathbb P(X\geq1)-\mathbb P(\chi(G)\leq k)\\
&\geq1-\mathbb EX-o(1)>0
\end{aligned}
$$

for all sufficiently large $n$. Hence at least one such $G$ contains no $K_{3,3}$ and has $\chi(G)>k$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [17H](../../17h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
