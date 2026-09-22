<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $A_2(N,\delta)$ for the largest number of codewords in a binary length-$N$ code with [minimum Hamming distance](../../../../../../minimum-distance-of-a-code.md) at least $\delta$. The volume of a [Hamming ball](../../../../../../hamming-ball.md) does not depend on its centre and is

$$
v_N(d)=\sum_{j=0}^d\binom Nj.
$$

For the [Hamming bound](../../../../../../hamming-bound.md), put $r=\lfloor(\delta-1)/2\rfloor$. The radius-$r$ [Hamming balls](../../../../../../hamming-ball.md) around distinct codewords are disjoint: a point belonging to two such balls would, by the [triangle inequality](../../../../../../triangle-inequality.md) for [Hamming distance](../../../../../../hamming-distance.md), put their centres at distance at most $2r<\delta$. Counting points in the binary cube therefore gives

$$
|C|v_N(r)\leq2^N.
$$

For the [Gilbert–Varshamov bound](../../../../../../gilbert-varshamov-bound.md), choose a code maximal under inclusion among those with [minimum Hamming distance](../../../../../../minimum-distance-of-a-code.md) at least $\delta$, for example by successively adding any allowable word. Its radius-$(\delta-1)$ [Hamming balls](../../../../../../hamming-ball.md) cover the cube. Otherwise an uncovered word would be at distance at least $\delta$ from every codeword and could be added, contradicting maximality. Thus

$$
2^N\leq |C|v_N(\delta-1).
$$

The lower bound is an existence assertion about a suitable code, while the upper bound holds for every such code. Together they give

$$
\boxed{\left\lceil\frac{2^N}{v_N(\delta-1)}\right\rceil
\leq A_2(N,\delta)\leq
\left\lfloor\frac{2^N}{v_N(\lfloor(\delta-1)/2\rfloor)}\right\rfloor.}
$$

Let $h_2(x)=-x\log_2x-(1-x)\log_2(1-x)$ be the [binary entropy](../../../../../../binary-entropy.md). For $\delta=\lfloor\lambda N\rfloor$,

$$
\frac{\delta-1}{N}\longrightarrow\lambda,\qquad
\frac{\lfloor(\delta-1)/2\rfloor}{N}\longrightarrow\frac{\lambda}{2}.
$$

The assumed [Hamming ball volume exponent](../../../../../../hamming-ball-volume-exponent.md) applies also to any integer radii $d_N$ with $d_N/N\to\theta\in(0,1/2)$. Indeed, for each small $\varepsilon>0$ these radii eventually lie between $\lfloor(\theta-\varepsilon)N\rfloor$ and $\lfloor(\theta+\varepsilon)N\rfloor$. [monotonicity](../../../../../../monotonic-function.md) of $v_N$ sandwiches its normalized logarithm between limits $h_2(\theta-\varepsilon)$ and $h_2(\theta+\varepsilon)$; continuity then lets $\varepsilon$ tend to zero. Consequently the [asymptotic Gilbert–Varshamov bound](../../../../../../asymptotic-gilbert-varshamov-bound.md) and [asymptotic Hamming bound](../../../../../../asymptotic-hamming-bound.md) have respective exponential scales

$$
\frac{2^N}{v_N(\delta-1)}=2^{N(1-h_2(\lambda))+o(N)},\qquad
\frac{2^N}{v_N(\lfloor(\delta-1)/2\rfloor)}
=2^{N(1-h_2(\lambda/2))+o(N)}.
$$

Equivalently, the optimal [code rate](../../../../../../code-rate.md) satisfies

$$
\boxed{1-h_2(\lambda)\leq
\liminf_{N\to\infty}\frac{\log_2A_2(N,\lfloor\lambda N\rfloor)}{N}
\leq\limsup_{N\to\infty}\frac{\log_2A_2(N,\lfloor\lambda N\rfloor)}{N}
\leq1-h_2(\lambda/2).}
$$

These are bounds on the rate, not a claim that the optimal rate has a known limit or equals either endpoint.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
