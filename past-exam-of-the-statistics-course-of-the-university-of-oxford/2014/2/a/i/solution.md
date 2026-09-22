<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For two simple [statistical hypotheses](../../../../../statistical-hypothesis.md) with joint [probability density functions](../../../../../probability-density-function.md) $g_0$ and $g_1$, fix a [significance level](../../../../../significance-level.md) $\alpha$. A [randomized statistical test](../../../../../randomized-statistical-test.md) $\varphi(x)$ is the conditional [probability](../../../../../probability.md) of rejection given the data. Choose $k\geq0$ and, if necessary, randomization on the equality set so that

$$
\varphi_*(x)=\begin{cases}1,&g_1(x)>kg_0(x),\\0,&g_1(x)<kg_0(x),\\\gamma(x)\in[0,1],&g_1(x)=kg_0(x),\end{cases}
\qquad \mathbb E_0\varphi_*=\alpha.
$$

The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) says that this is a [most powerful test](../../../../../most-powerful-test.md) among all tests with [test size](../../../../../size-of-a-statistical-test.md) at most $\alpha$:

$$
\boxed{\mathbb E_1\varphi\leq\mathbb E_1\varphi_*\quad\text{whenever}\quad\mathbb E_0\varphi\leq\alpha.}
$$

Thus the optimal ordering rejects where the alternative-to-null [likelihood ratio](../../../../../likelihood-ratio.md) is largest. On null-impossible observations with $g_1>0$, the rejection probability is one. Randomization is dispensable whenever an ordinary threshold already attains the required [test size](../../../../../size-of-a-statistical-test.md).

## ↑ Ancestors (13)

1. [I](../i.md)
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
