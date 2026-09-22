<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

We first show that a [continuous injection](../../../../continuous-injection.md) $j:S^1\to S^1$ must be [surjective](../../../../surjective-function.md). Otherwise its [image](../../../../image-of-a-function.md) misses a point $q$. [Stereographic projection](../../../../stereographic-projection.md) identifies $S^1\setminus\{q\}$ with $\mathbb R$, giving a [continuous injection](../../../../continuous-injection.md) $u:S^1\to\mathbb R$. The [extreme value theorem](../../../../extreme-value-theorem.md) supplies distinct points $p_-,p_+$ where $u$ attains its minimum $m$ and maximum $M$, with $m<M$ because $u$ is [injective](../../../../injective-function.md).

The two [circular arcs](../../../../circular-arc.md) from $p_-$ to $p_+$ each contain a point at which $u=(m+M)/2$, by the [intermediate value theorem](../../../../intermediate-value-theorem.md). Those points are distinct because they lie in the disjoint interiors of the two arcs. This contradicts [injectivity](../../../../injective-function.md), proving the claim about $j$.

Now suppose $F:S^2\to S^1$ were a [continuous injection](../../../../continuous-injection.md). Its restriction to the equatorial [circle](../../../../circle.md) $E=\{(x,y,0):x^2+y^2=1\}$ would be a [continuous injection](../../../../continuous-injection.md) from $S^1$ to itself, hence $F(E)=S^1$. The north pole $N=(0,0,1)$ is outside $E$, but $F(N)$ must equal $F(e)$ for some $e\in E$. This contradicts [injectivity](../../../../injective-function.md). Therefore

$$
\boxed{\text{there is no continuous injection }S^2\longrightarrow S^1.}
$$

## ↑ Ancestors (12)

1. [c](../c.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
