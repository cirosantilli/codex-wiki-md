<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [continuous function](../../../../../../continuous-function.md) $|h|$ attains a finite [maximum](../../../../../../maximum-of-a-subset-of-a-total-order.md) $M$ on $[a,b]$ by the [extreme value theorem](../../../../../../extreme-value-theorem.md). Additivity and the [triangle inequality](../../../../../../triangle-inequality.md) for the [Riemann integral](../../../../../../riemann-integral.md) imply, for any $x,y\in[a,b]$,

$$
\boxed{|H(y)-H(x)|=\left|\int_x^yh(t)\,dt\right|\leq M|y-x|.}
$$

For reversed endpoints, reverse the orientation of the [integral](../../../../../../integral-split.md) before taking its [absolute value](../../../../../../absolute-value.md). Given $\varepsilon>0$, choose $\delta=\varepsilon/(M+1)$. Then $|x-y|<\delta$ implies $|H(x)-H(y)|<\varepsilon$. Thus **$H$ is [continuous](../../../../../../continuous-function.md) on $[a,b]$**, including one-sided [continuity](../../../../../../continuous-function.md) at the endpoints; it is even [Lipschitz continuous](../../../../../../lipschitz-continuity.md). If $a=b$, the [function](../../../../../../function-split.md) is defined on one point and the conclusion is immediate.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
