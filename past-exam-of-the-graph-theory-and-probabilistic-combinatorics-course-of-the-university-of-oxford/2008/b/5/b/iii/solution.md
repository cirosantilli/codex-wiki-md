<h1 id="b/5/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For large $k$, choose

$$
n=\left\lceil 2^k\{k^2\log_e2+2k\log_e k\}\right\rceil.
$$

Using the two inequalities proved in part (a), the logarithm of the [union bound](../../../../../../boole-s-inequality.md) is at most

$$
k\log_e(en/k)-(n-k)2^{-k}.
$$

Now $\log_e(en/k)=k\log_e2+\log_e k+O(1)$, whereas $(n-k)2^{-k}=k^2\log_e2+2k\log_e k+o(1)$. Their difference is

$$
-k\log_e k+O(k)<0
$$

for all sufficiently large $k$. The existence criterion therefore applies. Since the chosen $n$ satisfies

$$
n=k^22^k(\log_e2)\left(1+O\!\left(\frac{\log k}{k}\right)\right),
$$

we obtain $\boxed{f(k)\le k^22^k(\log_e2)(1+o(1))}$, with the usual convention that the [tournament](../../../../../../tournament-graph-theory.md) has at least $k$ vertices. If orders below $k$ were permitted, the property would be vacuous there; the same upper bound remains valid but the extremal definition would be uninteresting.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
