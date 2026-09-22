<h1 id="21g/solution">Solution</h1>

↑ **Parent:** [21G](../21g.md)

The [Arzelà-Ascoli theorem](../../../../../arzela-ascoli-theorem.md) for $C([0,1])$ states that a family has compact closure in the uniform [norm](../../../../../norm.md) exactly when it is uniformly bounded and equicontinuous. To prove sufficiency, choose a countable dense set. From any [sequence](../../../../../sequence.md) of functions, successive subsequence extraction at each dense point and a diagonal selection give convergence at all those points. Given $\varepsilon>0$, [equicontinuity](../../../../../equicontinuity.md) gives a common $\delta$; cover the interval by finitely many $\delta$-balls centered at dense points. On a sufficiently late tail the functions differ by less than $\varepsilon/3$ at those finitely many centres, and [equicontinuity](../../../../../equicontinuity.md) makes each of the other two differences less than $\varepsilon/3$. Thus the selected subsequence is uniformly Cauchy. Completeness of $C([0,1])$ gives a continuous uniform limit. In a metric space this proves [compactness](../../../../../compact-space.md) of the closure. Conversely, a compact family has finite uniform $\varepsilon$-nets. The finitely many net functions are bounded and uniformly continuous; approximation by them gives a common bound and [equicontinuity](../../../../../equicontinuity.md) for the family. This proves both directions.

For $f\in S_N$, a positive interior maximum would have $f'=0$ and $f''\leq0$, contradicting $f''=f>0$. A negative interior minimum likewise contradicts $f''=f<0$. The endpoint bounds therefore give $|f|\leq N$ everywhere.

Now put $w=f'$. Differentiating the equation, using the stipulated third derivative, gives $w''=w+2ww'$. At an interior extremum of $w$, $w'=0$, so $w''=w$. The same maximum/minimum argument and the derivative endpoint bounds imply $|f'|=|w|\leq N$. Consequently $|f(x)-f(y)|\leq N|x-y|$ by the [mean value theorem](../../../../../mean-value-theorem.md). Thus $S_N$ is uniformly bounded and equicontinuous, and the theorem makes it relatively compact, hence **totally bounded in $C([0,1])$**. Its closure need not be asserted to remain thrice differentiable.

## ↑ Ancestors (10)

1. [21G](../21g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
