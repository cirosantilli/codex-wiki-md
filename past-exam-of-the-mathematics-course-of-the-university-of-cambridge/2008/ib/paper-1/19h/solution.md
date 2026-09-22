<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

Let $L$ be the last vertex visited for the first time, and assume $N\geq2$. Every vertex is eventually painted with probability one: from any position, $N-1$ consecutive clockwise steps visit the entire cycle, and the probability of such a block is $2^{-(N-1)}$. Thus the probability that coverage has not occurred after $m$ successive blocks is at most $(1-2^{-(N-1)})^m$, which tends to zero.

Fix $j\ne0$ and cut the cycle at $j$. Represent it as the path with positions $0,1,\ldots,N$, where the two endpoints both represent $j$ and the original starting vertex is at position $N-j$. Up to the first visit to $j$, the walk is a [simple symmetric random walk](../../../../../simple-symmetric-random-walk.md) on this path, killed at either endpoint. The event $L=j$ is precisely that it visits both $1$ and $N-1$ before being killed: travelling between these two positions visits all intermediate vertices, while visiting all non-$j$ vertices necessarily includes these two.

For $N\geq3$, first wait until the walk reaches one of $1,N-1$. This happens almost surely before it can reach an absorbing endpoint. If it reaches $1$ first, it must next reach $N-1$ before zero. The [gambler's ruin](../../../../../gambler-s-ruin.md) probability is $1/(N-1)$: the hitting probability $h(i)$ on $0\leq i\leq N-1$ satisfies

$$
h(0)=0,\quad h(N-1)=1,\quad h(i)=\tfrac12[h(i-1)+h(i+1)],
$$

so its successive differences are constant and $h(i)=i/(N-1)$. Starting at $1$ gives the stated probability. If the first endpoint reached is $N-1$, reflection of the path gives the same probability of reaching $1$ before $N$. The [Strong Markov property](../../../../../strong-markov-property.md) at the first such hit therefore gives $\mathbb P(L=j)=1/(N-1)$, independently of which endpoint was hit first and of the start position.

Consequently the [last visited vertex of a simple random walk on a cycle](../../../../../last-visited-vertex-of-a-simple-random-walk-on-a-cycle.md) has distribution

$$
\boxed{\mathbb P(L=0)=0,\qquad\mathbb P(L=j)=\frac1{N-1}\quad(1\leq j\leq N-1).}
$$

For $N=2$ the same formula follows directly since the only other post must be last. For $N=1$, painting the initial post already completes the task, so there is no subsequent last unpainted post.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
