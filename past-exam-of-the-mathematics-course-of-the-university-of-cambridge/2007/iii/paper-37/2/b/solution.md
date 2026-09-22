<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Expand $X^2=\sum_{A,B}I_AI_B$, where the sum is over ordered pairs of $k$-sets. If $|A\cap B|=l$, the two [cliques](../../../../../../clique-graph-theory.md) together require $2\binom k2-\binom l2$ different edges: precisely the edges within the overlap are counted twice. Therefore

$$
\mathbb E(I_AI_B)=p^{2\binom k2-\binom l2}.
$$

There are $\binom nk$ choices of $A$, then $\binom kl$ ways to choose the overlap and $\binom{n-k}{k-l}$ ways to choose the remaining vertices of $B$. It follows that

$$
\boxed{\mathbb EX^2=\sum_{l=0}^k\binom nk\binom kl\binom{n-k}{k-l}
 p^{2\binom k2-\binom l2}.}
$$

A [binomial coefficient](../../../../../../binomial-coefficient.md) is zero when its lower argument is outside its possible range. The term $l=k$ includes $A=B$ and equals $\mathbb EX$, as it should.

Now take the usual **fixed-$k$ interpretation** of the appearance assertion. For $k=1$, $X=n$ deterministically. For fixed $k\ge2$, the assumption $\mu_n\to\infty$ gives

$$
a_n=np^{(k-1)/2}\longrightarrow\infty,
$$

since $\mu_n\sim a_n^k/k!$. Eventually $p>0$. Subtracting $\mu_n^2$ in the second-moment formula, and using the identity that the overlap counts sum to the total number of ordered pairs, gives the [overlap formula for the variance of a clique count](../../../../../../overlap-formula-for-the-variance-of-a-clique-count.md):

$$
\frac{\operatorname{Var}X}{\mu_n^2}
=\sum_{l=2}^k\frac{\binom kl\binom{n-k}{k-l}}{\binom nk}
\left(p^{-\binom l2}-1\right).
$$

Overlaps of zero or one vertex have no shared edge and hence independent indicators, so their contributions vanish. For fixed $k$, the combinatorial coefficient in the $l$-th summand is $O_k(n^{-l})$. Moreover, because $p\le1$ and $l\le k$,

$$
n^{-l}p^{-l(l-1)/2}
=\bigl(np^{(l-1)/2}\bigr)^{-l}\le a_n^{-l}\longrightarrow0.
$$

There are only finitely many terms. Thus $\operatorname{Var}X/\mu_n^2\to0$. The [Chebyshev inequality](../../../../../../chebyshev-inequality.md) then gives

$$
\mathbb P(X=0)\le\mathbb P(|X-\mu_n|\ge\mu_n)
\le\frac{\operatorname{Var}X}{\mu_n^2}\longrightarrow0,
$$

proving the [fixed-size clique appearance threshold](../../../../../../fixed-size-clique-appearance-threshold.md):

$$
\boxed{\mathbb P(X\ge1)\longrightarrow1\quad\text{for fixed }k.}
$$

The fixed-size condition cannot simply be dropped. For $k=n-1$ and $p=1-(\log n)/n^2$,

$$
\mu_n=n\left(1-\frac{\log n}{n^2}\right)^{(n-1)(n-2)/2}
\sim\sqrt n\longrightarrow\infty.
$$

However the complement graph has a binomial number $J$ of missing edges with mean asymptotic to $\tfrac12\log n$ and [variance](../../../../../../variance-split.md) at most that mean. By the [Chebyshev inequality](../../../../../../chebyshev-inequality.md), $\mathbb P(J\ge2)\to1$. Conditional on $J\ge2$, choose two distinct missing edges uniformly; their endpoints are disjoint except with probability

$$
\frac{2(n-2)}{\binom n2-1}=O(n^{-1}).
$$

Thus with probability tending to one the complement has two disjoint edges. Deleting one vertex cannot remove both, so no $(n-1)$-clique exists. In this example $\mathbb P(X\ge1)\to0$, despite $\mu_n\to\infty$. This is [growing clique size can invalidate a first-moment appearance criterion](../../../../../../growing-clique-size-can-invalidate-a-first-moment-appearance-criterion.md); the exact second-moment identity remains valid for growing $k$, but the stated conclusion needs the conventional fixed-$k$ quantifier.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
