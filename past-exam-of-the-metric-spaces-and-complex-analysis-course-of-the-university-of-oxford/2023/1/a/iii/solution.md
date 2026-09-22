<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [iii](../iii.md)

First suppose $F$ is a [closed set](../../../../../closed-set.md). If $x\notin F$, the definition in part (ii) gives an [open ball](../../../../../open-ball.md) $B(x,r)$ disjoint from $F$. Thus every $y\in F$ has $d(x,y)\geq r$, and the [distance to a set](../../../../../distance-to-a-set.md) satisfies $\operatorname{dist}(x,F)\geq r>0$. Its contrapositive is the required implication.

Conversely, suppose that zero [distance to a set](../../../../../distance-to-a-set.md) forces membership. For $x\notin F$ we have $\operatorname{dist}(x,F)>0$. Choose $0<r<\operatorname{dist}(x,F)$. Then $B(x,r)\cap F=\varnothing$, proving $X\setminus F$ is an [open set](../../../../../open-set.md). Hence

$$
\boxed{F\text{ is closed}\ \Longleftrightarrow\ \forall x\in X,\quad\operatorname{dist}(x,F)=0\Rightarrow x\in F}.
$$

For $F=\varnothing$, use the extended-real convention $\inf\varnothing=+\infty$: both assertions hold, with the implication vacuous. Part (b) only uses nonempty sets, so all its [distances to a set](../../../../../distance-to-a-set.md) are ordinary finite real numbers.

## ↑ Ancestors (13)

1. [iii](../iii.md)
2. [a](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
