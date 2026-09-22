<h1 id="17f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $T$ be the number of [triangles](../../../../../../triangle-in-a-graph.md). Each edge $uv$ has at least  
$d(u)+d(v)-n$ [common neighbours](../../../../../../common-neighbour.md), and summing common-neighbour counts over [edges](../../../../../../edge-of-a-graph.md) counts every triangle three times. Hence

$$
\begin{aligned}
3T
&\geq\sum_{uv\in E}(d(u)+d(v)-n)\\
&=\sum_vd(v)^2-ne
\geq\frac{4e^2}{n}-ne
=e\left(\frac{4e}{n}-n\right).
\end{aligned}
$$

If $e>(1+\delta)n^2/4$, this is greater than  
$\delta en>\delta n^3/4$. Therefore

$$
\boxed{T>\frac{\delta}{12}n^3},
$$

so one may take $\varepsilon=\delta/12$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17F](../../17f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
