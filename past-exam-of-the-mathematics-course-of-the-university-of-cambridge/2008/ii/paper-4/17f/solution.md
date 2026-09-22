<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

Define the multicolour [graph Ramsey number](../../../../../graph-ramsey-number.md) $R_k(s_1,\ldots,s_k)$ as the least $n$ such that every colouring of the edges of the complete graph $K_n$ with $k$ colours contains, for some $i$, a complete subgraph on $s_i$ vertices all of whose edges have colour $i$.

Prove finiteness by induction on $\sum_i s_i$, temporarily allowing $s_i=1$. If some $s_i=1$, a single vertex supplies the required vacuous monochromatic clique, so the Ramsey number is one. Otherwise put $N_i=R_k(s_1,\ldots,s_i-1,\ldots,s_k)$, which is finite by induction, and take

$$
n=\sum_iN_i-k+2.
$$

Fix a vertex $v$ and partition its other $n-1$ vertices according to the colour of their edge to $v$. Some colour-$i$ class has at least $N_i$ vertices: if every class had at most $N_i-1$, their total would be at most $\sum_iN_i-k=n-2$. In that class the inductive property either gives a colour-$j$ clique of size $s_j$ with $j\ne i$, or a colour-$i$ clique of size $s_i-1$. In the latter case add $v$. Thus

$$
\boxed{R_k(s_1,\ldots,s_k)\leq\sum_iR_k(s_1,\ldots,s_i-1,\ldots,s_k)-k+2<\infty.}
$$

In particular the requested two-colour diagonal number is $R(s)=R_2(s,s)$, so it exists for every $s\geq2$.

Now colour each positive integer by its partition class, say there are $k$ classes, and take $m=R_k(3,\ldots,3)$. Colour the edge $ij$, $1\leq i<j\leq m$, by the class of $j-i$. There is a monochromatic triangle $a<b<c$. Its three differences $x=b-a$, $y=c-b$, $z=c-a$ are positive integers in one class, and

$$
\boxed{x+y=z.}
$$

This is the finite-Ramsey proof of the partition conclusion. The statement does not require $x$ and $y$ to be distinct.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
