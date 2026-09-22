<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [cumulative distribution function](../../../../cumulative-distribution-function.md) of the [uniform distribution](../../../../continuous-uniform-distribution.md) on $[0,1/n]$ is

$$
F_n(t)=\begin{cases}0,&t<0,\\nt,&0\leq t\leq1/n,\\1,&t>1/n.\end{cases}
$$

The constant zero has [cumulative distribution function](../../../../cumulative-distribution-function.md) $F(t)=\mathbf1_{[0,\infty)}(t)$. Its [continuity points](../../../../continuity-point.md) are precisely $t\ne0$. For fixed $t<0$, $F_n(t)=0=F(t)$; for fixed $t>0$, $F_n(t)=1=F(t)$ eventually. This proves [convergence in distribution](../../../../convergence-in-distribution.md) to zero directly from the definition.

Also, $\mathbb P(0\leq U_n\leq1/n)=1$. For every $\varepsilon>0$ and $n>1/\varepsilon$, $\mathbb P(|U_n|>\varepsilon)=0$. Hence

$$
\boxed{U_n\longrightarrow0\text{ both in distribution and in probability}.}
$$

The [convergence in probability](../../../../convergence-in-probability.md) conclusion holds for any realization of these [random variables](../../../../random-variable-split.md) on a common [probability space](../../../../probability-space-split.md); no [independence of random variables](../../../../independent-random-variables.md) is needed.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the probability course of the University of Oxford](../../../split.md)
5. [Probability course of the University of Oxford](../../../../probability-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
