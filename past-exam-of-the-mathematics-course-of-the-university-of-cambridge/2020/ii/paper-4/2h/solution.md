<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

A subset $A$ of a [metric space](../../../../../metric-space.md) is [nowhere dense](../../../../../nowhere-dense-set.md) when the interior of its closure is empty. One form of the [Baire category theorem](../../../../../baire-category-theorem.md) says that a nonempty [complete metric space](../../../../../complete-metric-space.md) cannot be a [countable union](../../../../../set-union.md) of nowhere dense closed sets; equivalently, a countable intersection of dense open sets is dense.

Fix $\varepsilon>0$ and work in the complete interval $[1,2]$. For $N\geq1$ define the closed set

$$
E_N=\{x\in[1,2]: |f(nx)|\leq\varepsilon\text{ for every }n\geq N\}.
$$

The sets are closed by the [continuity](../../../../../continuous-function.md) of $f$, and the assumed [pointwise convergence](../../../../../pointwise-convergence.md) gives $[1,2]=\bigcup_NE_N$. The [Baire category theorem](../../../../../baire-category-theorem.md) therefore gives an $N$ and a nonempty open interval $(a,b)\subseteq[1,2]$ contained in $E_N$.

The intervals $[na,nb]$ overlap once $(n+1)a\leq nb$, which holds for every sufficiently large [natural number](../../../../../natural-number.md) $n$. Their union consequently contains a half-line. Every sufficiently large $t$ can therefore be written as $t=nx$ with $n\geq N$ and $x\in(a,b)$, and then $|f(t)|=|f(nx)|\leq\varepsilon$. Since $\varepsilon$ was arbitrary, $f(t)\to0$ as $t\to\infty$.

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
