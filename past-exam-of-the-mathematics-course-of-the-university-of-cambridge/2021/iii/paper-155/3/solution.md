<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Bourgain embedding theorem](../../../../../bourgain-embedding-theorem.md) states that every $n$-point metric space embeds into a Hilbert space with distortion at most $C\log n$; the random-subset construction may be taken to have dimension $O((\log n)^2)$.

We use the following finite [Fréchet embedding](../../../../../frechet-embedding.md) lemma. For every integer $q\geq2$, an $n$-point metric space $X$ has subsets $A_1,\ldots,A_k$ such that

$$
k\leq Cq n^{1/q}\log n
$$

and, for every $x,y\in X$, some $A_i$ satisfies

$$
|d(x,A_i)-d(y,A_i)|\geq\frac{d(x,y)}{2q-1}.
$$

Here is the probabilistic proof. Put $\vartheta=n^{-1/q}$. For every level $i=1,\ldots,q$, independently form

$$
m=\lceil24\vartheta^{-1}\log n\rceil
$$

random subsets $A_{i,j}$ by including each point with probability $p_i=\min\{1/2,n^{-i/q}\}$.

Fix $x,y$ and put $\Delta=d(x,y)/(2q-1)$. Form $q+1$ open balls $B_0,\ldots,B_q$ by taking $B_t$ to have radius $t\Delta$ and center $x$ for even $t$ and $y$ for odd $t$. Consecutive balls are disjoint because their radii sum to at most $(2q-1)\Delta=d(x,y)$. Partition the cardinality interval $[1,n]$ into

$$
[n^{(i-1)/q},n^{i/q}],
\qquad i=1,\ldots,q.
$$

Among the $q+1$ cardinalities $|B_t|$, either two consecutive ones lie in one interval, or some consecutive pair decreases. In either case there are $i,t$ such that, after orienting the pair appropriately,

$$
|B_t|\geq n^{(i-1)/q},
\qquad |B_{t+1}|\leq n^{i/q}.
$$

At level $i$, a random set hits $B_t$ with probability at least $\vartheta/3$ and misses the disjoint $B_{t+1}$ with probability at least $1/4$. These events are independent, and when both occur the two distance-to-set values differ by at least $\Delta$. Thus one sample succeeds with probability at least $\vartheta/12$. All $m$ samples at that level fail with probability at most

$$
(1-\vartheta/12)^m\leq n^{-2}.
$$

A union bound over the fewer than $n^2/2$ unordered pairs leaves a simultaneous successful choice. There are $qm\leq Cqn^{1/q}\log n$ coordinates, proving the lemma.

Define

$$
F:X\longrightarrow\ell_\infty^k,
\qquad F(x)=(d(x,A_i))_{i=1}^k.
$$

Every distance-to-set coordinate is one-Lipschitz, while the lemma supplies the lower bound. Hence

$$
\frac1{2q-1}d(x,y)\leq\|F(x)-F(y)\|_\infty\leq d(x,y),
$$

proving the [Low-dimensional Frechet embedding into linfinity](../../../../../low-dimensional-frechet-embedding-into-linfinity.md).

Take $q=\lceil\log n\rceil$. Then $n^{1/q}\leq e$, $k=O((\log n)^2)$, and the distortion into $\ell_\infty^k$ is $O(\log n)$. Since

$$
\|v\|_\infty\leq\|v\|_2\leq\sqrt{k}\|v\|_\infty,
$$

the identity $\ell_\infty^k\to\ell_2^k$ has distortion $O(\log n)$. Composition gives

$$
\boxed{c_2(n)=O((\log n)^2)}.
$$

Finally let a $d$-regular expander $G$ embed into $\ell_\infty^k$ with distortion at most $\alpha$. For $1<p<\infty$, the identity

$$
\ell_\infty^k\longrightarrow\ell_p^k
$$

has distortion at most $k^{1/p}$. Therefore the assumed lower bound gives

$$
\frac{C\log n}{p}\leq c_p(G)\leq\alpha k^{1/p}.
$$

For $k\geq e^2$, choose $p=\log k$, so $k^{1/p}=e$ and

$$
\log k\geq\frac C{e\alpha}\log n.
$$

Adjusting the constant handles bounded $k$, and exponentiation proves the [Dimension lower bound for an expander embedded in linfinity](../../../../../dimension-lower-bound-for-an-expander-embedded-in-linfinity.md)

$$
\boxed{k\geq n^{c/\alpha}},
$$

where $c>0$ depends only on $d$ and $h$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 155](../../paper-155-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
