<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [first-step analysis](../../../../../first-step-analysis.md) gives $h_0=1$ and, for $k\geq1$,

$$
h_k=p h_{k+1}+q h_{k-1}.
$$

The [minimal nonnegative solution for hitting probabilities](../../../../../hitting-probability-is-the-minimal-nonnegative-harmonic-extension.md) theorem states that the probability of ever hitting a target is the pointwise smallest nonnegative solution of this transition recurrence with value one at the target. It follows by comparing any such solution with the probabilities of hitting within $n$ steps, then taking their increasing limit.

The characteristic equation $pr^2-r+q=0$ has distinct roots $1$ and $\beta=q/p\in(0,1)$. Hence every solution on the nonnegative integers with boundary value one has the form

$$
g_k=A+(1-A)\beta^k.
$$

If it is nonnegative for all $k$, taking $k\to\infty$ forces $A\geq0$, and therefore $g_k-\beta^k=A(1-\beta^k)\geq0$. The candidate $g_k=\beta^k$ is itself nonnegative and satisfies the recurrence and boundary value. It is consequently the minimal solution, giving the [biased random walk hitting probability](../../../../../biased-random-walk-hitting-probability.md)

$$
\boxed{h_k=\left(\frac{1-p}{p}\right)^k,\qquad k>0;\qquad
\beta=\frac{1-p}{p}.}
$$

On the negative half-line the already established values $h_k=1$ satisfy the same recurrence away from zero. No unproved boundary condition at infinity has been imposed.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
