<h1 id="19h/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Two cuts give the upper bounds

$$
\delta^*(x)\leq x+5
$$

from the source cut, and

$$
\delta^*(x)\leq14
$$

from the cut whose source side is

$$
S=\{s,r,a,b,c,d,f\}.
$$

The latter cut crosses the edges $ce,de,dg,ft$, of respective capacities $3,3,2,6$.

At $x=0$, a flow of value $5$ is

$$
sb=bd=5,
\qquad de=et=3,
\qquad dg=gt=2.
$$

At $x=9$, a flow of value $14$ is given by

$$
\begin{array}{c|rrrrrrrrrrrrr}
\text{edge}&sr&sb&rc&ra&ac&bd&cf&ce&de&dg&et&ft&gt\\ \hline
\text{flow}&9&5&6&3&3&5&6&3&3&2&6&6&2.
\end{array}
$$

For $0\leq x\leq9$, take the convex combination of these two flows with weights $1-x/9$ and $x/9$. It is feasible at capacity $x$ and has value $5+x$. For $x\geq9$, the second flow remains feasible and has value $14$. The two cut bounds are therefore attained, and the [parametric maximum flow with one source capacity](../../../../../../../parametric-maximum-flow-with-one-source-capacity.md) is

$$
\boxed{
\delta^*(x)=\min\{x+5,14\}
=\begin{cases}
x+5,&0\leq x\leq9,\\
14,&x\geq9.
\end{cases}}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [19H](../../../19h.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ib](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
