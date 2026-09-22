<h1 id="e/e4/solution">Solution</h1>

↑ **Parent:** [E4](../e4.md)

A [sequentially compact space](../../../../sequentially-compact-space.md) is one in which every sequence has a subsequence converging to a point of the space. A [limit point](../../../../limit-point.md) $\ell$ of $S$ means every open ball around $\ell$ meets $S\setminus\{\ell\}$.

In a compact [metric space](../../../../metric-space.md), a sequence with a finite set of values has a constant subsequence. If its value set is infinite and had no [limit point](../../../../limit-point.md), each point of the space would have a neighbourhood containing at most one point of that value set. A finite subcover would then make the value set finite, a contradiction. It therefore has a [limit point](../../../../limit-point.md) in the space, and the permitted subsequence result gives a convergent subsequence. This proves sequential compactness.

For the remaining assertions assume the [compact space](../../../../compact-space.md) is nonempty, as required for a fixed-point claim. The displacement function $q(x)=d(f(x),x)$ is continuous by the stated continuity of the metric and of $f$. The [extreme value theorem](../../../../extreme-value-theorem.md) gives a minimum $\delta=q(p)$. If $\delta>0$, then $p\neq f(p)$, and strict decrease of distances implies

$$
q(f(p))=d(f^2(p),f(p))<d(f(p),p)=\delta,
$$

contradicting minimality. Thus $\delta=0$ and $p$ is a [fixed point](../../../../fixed-point.md). Two distinct fixed points would satisfy $d(p,q)=d(f(p),f(q))<d(p,q)$, also impossible. Hence the [fixed point](../../../../fixed-point.md) is unique.

On the noncompact real line, take

$$
\boxed{f(x)=\log(1+e^x).}
$$

Its derivative $e^x/(1+e^x)$ is strictly between zero and one. The [mean value theorem](../../../../mean-value-theorem.md) therefore gives $|f(x)-f(y)|<|x-y|$ for each distinct pair. Yet $f(x)-x=\log(1+e^{-x})>0$, so it has no [fixed point](../../../../fixed-point.md). Compactness, rather than merely pointwise strict shrinkage, supplies attainment of a zero displacement in the preceding proof.

## ↑ Ancestors (12)

1. [E4](../e4.md)
2. [E](../../e.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
