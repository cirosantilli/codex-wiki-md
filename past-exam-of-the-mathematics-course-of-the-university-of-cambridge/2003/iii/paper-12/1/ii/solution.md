<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $X_t$ count $t$-[cliques](../../../../../../clique-graph-theory.md), and put $\mu_t=\binom ntp^{\binom t2}$. Since $\mu_{r+1}\to0$, the [Markov inequality](../../../../../../markov-inequality.md) gives $\Pr(X_{r+1}>0)\to0$. Any larger [clique](../../../../../../clique-graph-theory.md) contains an $(r+1)$-clique, so it remains to prove $X_r>0$ [with high probability](../../../../../../with-high-probability.md).

We give the required [growing-clique overlap bound](../../../../../../growing-clique-overlap-bound.md) explicitly. Set $\mu=\mu_r$ and, for $2\leq s\leq r$,

$$
a_s=\frac{\binom rs\binom{n-r}{r-s}}{\binom nr},\qquad T_s=a_sp^{-\binom s2}.
$$

The quantity $a_s$ is the [probability](../../../../../../probability.md) that a uniformly chosen $r$-set overlaps a fixed $r$-set in exactly $s$ [vertices](../../../../../../vertex-graph-theory.md). Two clique indicators share exactly $\binom s2$ edge requirements, so their joint-to-product ratio is $p^{-\binom s2}$. Overlap zero or one gives independence. Hence the [overlap formula for the variance of a clique count](../../../../../../overlap-formula-for-the-variance-of-a-clique-count.md) implies

$$
\frac{\operatorname{Var}X_r}{\mu^2}=\sum_{s=2}^r a_s\bigl(p^{-\binom s2}-1\bigr)\leq\sum_{s=2}^r T_s.
$$

We must bound this sum with $r$ allowed to grow.

Eventually $\mu_r\geq1$ and $\mu_{r+1}\leq1$. Using $(n/t)^t\leq\binom nt\leq(en/t)^t$, these inequalities give

$$
p^{-1}\leq(en/r)^{2/(r-1)},\qquad p\leq((r+1)/n)^{2/r}.
$$

For $2\leq s\leq r/2$, a [union bound](../../../../../../boole-s-inequality.md) over the $s$ selected shared vertices gives $a_s\leq\binom rs(r/(n-r))^s$. Put $a=(s-1)/(r-1)<1/2$. Since $n\geq r^3$ and $n-r\geq n/2$,

$$
T_s\leq\left[\frac{2er^2}{sn}(en/r)^a\right]^s\leq\left[\frac{2e^2}{s}r^{-1+2a}\right]^s\leq\left(\frac{2e^2}{s}\right)^s.
$$

For each fixed $s$, the first bound tends to zero if $r$ stays bounded, because its power of $n$ is negative. If $r\to\infty$, the middle bound tends to zero because $a\to0$. Thus each fixed-$s$ term tends to zero along arbitrary admissible sequences. The bounding [series](../../../../../../series-mathematics.md) $\sum_{s\geq2}(2e^2/s)^s$ converges. Splitting at a fixed large index, then taking $n\to\infty$ and the index to infinity, proves that the entire lower-half sum is $o(1)$.

For the upper half write $s=r-j$. The exact diagonal comparison is

$$
T_{r-j}=\frac1\mu\binom rj\binom{n-r}j p^{j(2r-j-1)/2},\qquad T_r=\frac1\mu.
$$

For $1\leq j\leq r/2$, the second bound on $p$ gives

$$
\mu T_{r-j}\leq\left[\frac{e^2r(r+1)^2}{nj^2}\left(\frac n{r+1}\right)^{(j+1)/r}\right]^j\leq\left[\frac{2e^2r^{2(j+1)/r}}{j^2}\right]^j.
$$

The last inequality uses $n\geq r^3$: the exponent of $n$ in the bracket is negative, so substituting $n=r^3$ bounds it above. Uniformly for this range of $j$, $r^{2(j+1)/r}\leq9j$. Indeed $r^{2/r}\leq3$, and concavity of $\log(3j)-(2j/r)\log r$, checked at $j=1$ and $j=r/2$, gives $r^{2j/r}\leq3j$. It follows that

$$
\sum_{s>r/2}T_s\leq\frac1\mu\left[1+\sum_{j\geq1}\left(\frac{18e^2}{j}\right)^j\right]=O(\mu^{-1})=o(1).
$$

Thus $\operatorname{Var}X_r=o(\mu^2)$. The [second moment method](../../../../../../second-moment-method.md) gives $\Pr(X_r=0)\to0$. Combining this with the absence of larger [cliques](../../../../../../clique-graph-theory.md) proves

$$
\boxed{\Pr\bigl(\text{clique number of }G_{n,p}=r\bigr)\longrightarrow1.}
$$

The restriction on $r$ is used in both overlap ranges; divergence of a [clique count in a binomial random graph](../../../../../../clique-count-in-a-binomial-random-graph.md) alone would not suffice for arbitrary growing $r$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
