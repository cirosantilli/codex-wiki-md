<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $S=T_b\wedge T_{-a}$ and $p=\mathbb P(T_b<T_{-a})$. Set $R=\max(a,b)$. The exit time $S$ from $(-a,b)$ is at most the exit time from $(-R,R)$, so part (ii) gives $\mathbb ES<\infty$. Continuity ensures that exactly one of the two different boundary levels is reached at $S$.

The stopped [local martingale](../../../../../local-martingale.md) $e^{X_{t\wedge S}}$ lies in $[e^{-a},e^b]$, hence is a [uniformly integrable martingale](../../../../../uniformly-integrable-martingale.md). The [optional sampling theorem](../../../../../optional-sampling-theorem-for-a-supermartingale.md), justified at the terminal time also by [bounded convergence theorem](../../../../../bounded-convergence-theorem.md), gives

$$
1=\mathbb Ee^{X_S}=pe^b+(1-p)e^{-a}.
$$

Thus the [boundary hitting probability from a diffusion scale function](../../../../../boundary-hitting-probability-from-a-diffusion-scale-function.md) is

$$
\boxed{\mathbb P(T_b<T_{-a})
=\frac{1-e^{-a}}{e^b-e^{-a}}
=\frac{e^a-1}{e^{a+b}-1}.}
$$

For integer $n\to\infty$, the events $\{T_b<T_{-n}\}$ increase to $\{T_b<\infty\}$. Indeed, on any path with finite $T_b$, continuity makes the path bounded below on $[0,T_b]$, so some lower barrier $-n$ has not yet been hit. The reverse inclusion is immediate. Taking the limit in the displayed probability gives

$$
\boxed{\mathbb P(T_b<\infty)=e^{-b}\qquad(b>0).}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations course of the University of Oxford](../../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
