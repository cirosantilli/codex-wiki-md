<h1 id="a/1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take $S=T(B_X)$. A [bounded linear operator](../../../../../continuous-linear-operator.md) is compact exactly when the closure of this set is compact. In a [complete metric space](../../../../../complete-metric-space.md) this is equivalent to its being [totally bounded](../../../../../totally-bounded-space.md).

If $T$ is compact, choose a finite $\varepsilon$-net $z_1,\ldots,z_m$ for $T(B_X)$ and let $Y$ be their span. Then $\operatorname{dist}(Tx,Y)<\varepsilon$ for $\|x\|\leq1$, giving $\|\pi_YT\|\leq\varepsilon$.

Conversely, fix $\delta>0$ and take $Y$ with $\|\pi_YT\|\leq\delta/4$. For every $x\in B_X$ choose $y_x\in Y$ with $\|Tx-y_x\|<\delta/2$. These approximants satisfy $\|y_x\|\leq\|T\|+\delta/2$, so form a bounded subset of a finite-dimensional space and have a finite $\delta/2$-net. The same centers give a finite $\delta$-net for $T(B_X)$. Thus it is [totally bounded](../../../../../totally-bounded-space.md) and $T$ is compact. In particular

$$
\boxed{T\text{ compact}\iff\forall\varepsilon>0\ \exists\dim Y<\infty:\ \|\pi_YT\|\leq\varepsilon.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
