<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $C=M_0^{1-\theta}M_1^\theta$. Since $p<\infty$, choose [simple functions](../../../../../../simple-function.md) $f_n$ of finite-measure support with $f_n\to f$ in $L^p$. These belong to both endpoint domain spaces. The given simple-function estimate applies also to their differences, so

$$
\|Tf_n-Tf_m\|_q\leq C\|f_n-f_m\|_p.
$$

By [completeness of Lp spaces](../../../../../../completeness-of-lp-spaces.md), including $L^\infty$, there is $u\in L^q$ with $Tf_n\to u$ in $L^q$. Taking limits of the simple-function bound yields $\|u\|_q\leq C\|f\|_p$.

It remains to identify $u$ with the already defined $Tf$, rather than just define an unrelated extension. Write $X=L^{p_0}+L^{p_1}$ and $Y=L^{q_0}+L^{q_1}$ with their sum [norms](../../../../../../norm.md). The endpoint estimates imply

$$
\|Tv\|_Y\leq\max(M_0,M_1)\|v\|_X.
$$

Indeed, split $v=v_0+v_1$, bound the two images in their endpoint [norms](../../../../../../norm.md), and take the infimum over all splits. Part (i) gives $\|f_n-f\|_X\leq2\|f_n-f\|_p$, hence $Tf_n\to Tf$ in $Y$.

The inclusion $L^q\subseteq Y$ is also continuous. For distinct finite endpoints this is the same threshold argument as part (i), after ordering the endpoints. If the larger endpoint is infinity, splitting at $a=\|v\|_q$ bounds both the lower endpoint [norm](../../../../../../norm.md) of the large-value part and the [supremum norm](../../../../../../supremum-norm.md) of the small-value part by $\|v\|_q$. If the endpoints coincide, the inclusion is immediate. Thus $Tf_n\to u$ also in $Y$. Uniqueness of limits in the sum [norm](../../../../../../norm.md) gives $u=Tf$ [almost everywhere](../../../../../../almost-everywhere.md). Consequently the [Riesz-Thorin theorem](../../../../../../riesz-thorin-theorem.md) estimate extends as

$$
\boxed{\|Tf\|_q\leq M_0^{1-\theta}M_1^\theta\|f\|_p
\quad\text{for every }f\in L^p.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
