<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work in the [Banach space](../../../../banach-space-split.md) $C([0,1])$ with its [supremum norm](../../../../supremum-norm.md), and take the nonempty closed bounded convex set $M=\{u:100\leq u(t)\leq121\text{ for all }t\}$. Define

$$
(Tu)(t)=101+\int_0^t\bigl(\sqrt{|u(s)|}+1\bigr)\,ds.
$$

For $u\in M$ the absolute value is unnecessary, and $\boxed{101\leq Tu(t)\leq101+12=113\leq121}$. Thus $T:M\to M$. Also, for $a,b\geq100$,

$$
|\sqrt a-\sqrt b|=\frac{|a-b|}{\sqrt a+\sqrt b}\leq\frac1{20}|a-b|,
$$

so $\|Tu-Tv\|_\infty\leq\tfrac1{20}\|u-v\|_\infty$ and in particular $T$ is continuous.

The image is uniformly bounded, and $|Tu(t)-Tu(s)|\leq12|t-s|$, so it is [equicontinuous](../../../../equicontinuity.md). The [Arzelà-Ascoli theorem](../../../../arzela-ascoli-theorem.md) says that a uniformly bounded equicontinuous family in $C([0,1])$ has [relatively compact](../../../../relatively-compact-subset.md) [closure](../../../../closure-topology.md) in the uniform norm. Hence $T$ is compact, and the [Schauder fixed-point theorem](../../../../schauder-fixed-point-theorem.md) supplies $\boxed{u=Tu}$, the required solution. In fact the displayed contraction estimate also lets the [contraction mapping theorem](../../../../contraction-mapping-theorem.md) give uniqueness within $M$ and convergence of the corresponding [Picard iteration](../../../../picard-iteration.md). The initial constant here is the printed integer $101$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
