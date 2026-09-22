<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $r\geq0$, [Lebesgue measure](../../../../../../../lebesgue-measure.md) of the ball is $v_dr^d$, so the [Poisson random measure](../../../../../../../poisson-random-measure.md) gives $N_r\sim\operatorname{Poisson}(v_dr^d)$ and

$$
\mathbb P(N_r=0)=e^{-v_dr^d}.
$$

By monotonicity of the balls, the set of radii with no points is an interval starting at zero. Thus $\{R\geq r\}=\{N_r=0\}$: if all smaller balls are empty then their union, the open ball of radius $r$, is empty; if that ball is empty then its radius belongs to the defining set. We obtain

$$
\mathbb P(R\geq r)=e^{-v_dr^d}.
$$

The continuous tail gives $\mathbb P(R=0)=0$ and $\mathbb P(R=\infty)=0$. Differentiating the [cumulative distribution function](../../../../../../../cumulative-distribution-function.md) gives the [probability density function](../../../../../../../probability-density-function.md)

$$
\boxed{f_R(r)=d v_d r^{d-1}e^{-v_dr^d}\mathbf1_{\{r>0\}}.}
$$

The substitution $u=v_dr^d$ proves that this density integrates to one; equivalently $v_dR^d$ has the unit-rate [exponential distribution](../../../../../../../exponential-distribution.md). This is the first-neighbour case of the [Kth-nearest-neighbour distance in a homogeneous Poisson point process](../../../../../../../kth-nearest-neighbour-distance-in-a-homogeneous-poisson-point-process.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
