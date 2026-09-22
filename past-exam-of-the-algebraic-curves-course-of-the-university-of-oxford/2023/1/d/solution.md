<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $d_i=\deg C_i$. Under the [reduced plane curve](../../../../reduced-plane-curve.md) convention, the distinct [irreducible components](../../../../irreducible-component.md) have $\sum_i d_i=d$. Away from intersections with other components, a point of $C_i$ is nonsingular on the union exactly when it is nonsingular on $C_i$. For example, a local equation of the union is the equation of $C_i$ multiplied by a nonvanishing factor. At an intersection of two components, differentiating their product makes every first [partial derivative](../../../../partial-derivative.md) vanish. Therefore

$$
\operatorname{Sing}(C)=\bigcup_i\operatorname{Sing}(C_i)\ \cup\ \bigcup_{i<j}(C_i\cap C_j).
$$

Part (b) bounds the number of [singular points](../../../../singular-point-of-an-algebraic-variety.md) of $C_i$ by $d_i(d_i-1)/2$. For each distinct pair of [irreducible components](../../../../irreducible-component.md), [Bézout's theorem](../../../../bezout-s-theorem.md) bounds the number of distinct intersections by $d_id_j$. The [cardinality](../../../../cardinality.md) of a union is at most the sum of the [cardinalities](../../../../cardinality.md), even if some points have been counted several times. Hence

$$
\begin{aligned}
\#\operatorname{Sing}(C)
&\leq\sum_i\frac{d_i(d_i-1)}2+\sum_{i<j}d_id_j\\
&=\frac12\left(\left(\sum_i d_i\right)^2-\sum_i d_i\right)
=\boxed{\frac{d(d-1)}2}.
\end{aligned}
$$

The reduced convention matters. If one instead allows the equation $L^2=0$ as a nonreduced curve and uses its equation to test singularity, every point on its supporting line has vanishing first [partial derivatives](../../../../partial-derivative.md). A finite bound would then be false.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic curves course of the University of Oxford](../../../split.md)
5. [Algebraic curves course of the University of Oxford](../../../../algebraic-curves-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
