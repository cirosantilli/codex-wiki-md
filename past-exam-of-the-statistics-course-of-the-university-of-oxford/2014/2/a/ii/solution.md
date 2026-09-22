<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a random sample, write $g_j(x)=\prod_{i=1}^nf(x_i;\theta_j)$, $j=0,1$, for its joint [probability density functions](../../../../../probability-density-function.md). Let $\varphi$ be any competing [statistical test](../../../../../statistical-test.md) of level at most $\alpha$. Pointwise,

$$
(\varphi_* -\varphi)(g_1-kg_0)\geq0.
$$

Indeed, where $g_1>kg_0$, $\varphi_*=1\geq\varphi$; where $g_1<kg_0$, $\varphi_*=0\leq\varphi$, so both factors have the same sign. On the equality set the product is zero, regardless of randomization. Integrate over the joint sample space using its ordinary volume measure:

$$
\begin{aligned}
0&\leq\int(\varphi_* -\varphi)(g_1-kg_0)\,dx\\
&=\mathbb E_1\varphi_* -\mathbb E_1\varphi-k(\mathbb E_0\varphi_* -\mathbb E_0\varphi).
\end{aligned}
$$

Since $k\geq0$ and $\mathbb E_0\varphi_* =\alpha\geq\mathbb E_0\varphi$,

$$
\boxed{\mathbb E_1\varphi_* -\mathbb E_1\varphi\geq k(\alpha-\mathbb E_0\varphi)\geq0.}
$$

This proves maximal [power](../../../../../power.md). A continuous sample distribution does not itself guarantee that the equality set of the [likelihood ratio](../../../../../likelihood-ratio.md) has zero probability; allowing randomization there makes the proof valid in that case too.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
