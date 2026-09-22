<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

Let the win [probabilities](../../../../../probability.md) in games 1,2,3 be $u,v,w$. [Independence](../../../../../independent-random-variables.md) makes a prescribed result pattern the product of its three win/loss [probabilities](../../../../../probability.md). Taking a complement for event (a), [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) for overlapping pairs in (b) and (c), and disjoint exact-two patterns in (d) and (e), gives

$$
\begin{array}{c|l}
\text{event}&\text{probability}\\\hline
(a)&1-(1-u)(1-v)(1-w)\\
(b)&uv+vw+uw-2uvw\\
(c)&uv+vw-uvw\\
(d)&uv(1-w)+(1-u)vw\\
(e)&uv(1-w)+(1-u)vw+u(1-v)w
\end{array}
$$

For (b), a three-win outcome is counted three times in the pair sum and must be counted once, so subtract twice its [probability](../../../../../probability.md). For (c), only the overlapping pairs 12 and 23 are allowed, so subtract the three-win intersection once. For (d), the two allowed exact patterns are 110 and 011. For (e), add 101 as well.

Substituting $(u,v,w)=(q,p,q)$ and $(p,q,p)$ gives the complete comparison:

$$
\boxed{\begin{array}{c|c|c|c}
& DMD&MDM&\text{maximizing order}\\\hline
(a)&1-(1-q)^2(1-p)&1-(1-p)^2(1-q)&MDM\\
(b)&2pq+q^2-2pq^2&2pq+p^2-2p^2q&MDM\\
(c)&pq(2-q)&pq(2-p)&DMD\\
(d)&2pq(1-q)&2pq(1-p)&DMD\\
(e)&2pq+q^2-3pq^2&2pq+p^2-3p^2q&MDM
\end{array}}
$$

For (a) and (b), the differences $P_{MDM}-P_{DMD}$ are respectively $(p-q)(1-p)(1-q)>0$ and $(p-q)(p+q-2pq)>0$. For (c) and (d), the differences $P_{DMD}-P_{MDM}$ are $pq(p-q)>0$ and $2pq(p-q)>0$. For (e), $P_{MDM}-P_{DMD}=(p-q)(p+q-3pq)>0$ by the additional hypothesis. Thus all maximizing orders follow with strict inequalities.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
