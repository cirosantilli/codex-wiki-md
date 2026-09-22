<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the [edge-isoperimetric theorem for binary initial segments](../../../../../../edge-isoperimetric-theorem-for-binary-initial-segments.md) by counting edges of the [induced subgraph](../../../../../../induced-subgraph.md). Identify each vertex of the [hypercube graph](../../../../../../hypercube-graph.md) $Q_n$ with an integer $j\in\{0,\ldots,2^n-1\}$ via its binary digits; the [binary order on the discrete cube](../../../../../../binary-order-on-the-discrete-cube.md) is increasing integer order. Let $s_2(j)$ be its [Hamming weight](../../../../../../hamming-weight.md), and set

$$
F(a)=\sum_{j=0}^{a-1}s_2(j),\qquad F(0)=0.
$$

A vertex $j$ in the initial segment has exactly $s_2(j)$ neighbours of smaller label, obtained by changing a one to zero. Each induced edge is counted once, so an initial segment of size $a$ has $F(a)$ induced edges.

The arithmetic ingredient is the [binary digit-sum inequality](../../../../../../binary-digit-sum-inequality.md)

$$
F(a+b)\geq F(a)+F(b)+\min(a,b)\qquad(a,b\geq0).
$$

Here is a proof, including the parity cases needed for arbitrary sizes. Pair the numbers $2j,2j+1$ to obtain

$$
F(2r)=2F(r)+r,\qquad F(2r+1)=F(r)+F(r+1)+r.
$$

Write $G(a,b)=F(a+b)-F(a)-F(b)$ and induct on $a+b$, assuming $a\leq b$. If $a=0$, the claim is immediate. Otherwise the recurrences express $G(a,b)-a$ as follows:

$$
\begin{array}{c|c|c}
(a,b)&\text{restriction}&G(a,b)-a\\\hline
(2s,2t)&s\leq t&2G(s,t)-2s\\
(2s,2t+1)&s\leq t&G(s,t)+G(s,t+1)-2s\\
(2s+1,2t)&s+1\leq t&G(s,t)+G(s+1,t)-(2s+1)\\
(2s+1,2t+1)&s\leq t&G(s,t+1)+G(s+1,t)-2s
\end{array}
$$

Every pair on the right has smaller total size. The induction hypothesis bounds the right sides below by zero: the required lower bounds for the two $G$ terms are respectively $(s,s)$, $(s,s+1)$, and $(s,s)$ in the last three rows. This establishes the [binary digit-sum inequality](../../../../../../binary-digit-sum-inequality.md).

Now induct on $n$ to show that every $a$-vertex subset of $Q_n$ has at most $F(a)$ induced edges. The zero-dimensional case is immediate. Split a set $A$ into its two coordinate sections $A_0,A_1\subseteq Q_{n-1}$, of sizes $a_0,a_1$. By induction the edges within the sections number at most $F(a_0)+F(a_1)$. The edges between the sections form a [matching in a graph](../../../../../../matching-graph-theory.md), so at most $\min(a_0,a_1)$ are present. Hence

$$
e(A)\leq F(a_0)+F(a_1)+\min(a_0,a_1)\leq F(a_0+a_1).
$$

Finally, $Q_n$ is a [regular graph](../../../../../../regular-graph.md) of degree $n$, so its [edge boundary in a graph](../../../../../../edge-boundary-in-a-graph.md) satisfies $|\partial_eA|=n|A|-2e(A)$. For the binary initial segment $C$, equality $e(C)=F(|A|)$ holds. Therefore

$$
\boxed{|\partial_eA|\geq n|A|-2F(|A|)=|\partial_eC|.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
