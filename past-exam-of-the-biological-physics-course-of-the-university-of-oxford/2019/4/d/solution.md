<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume identical dwell states and memoryless forward/backward exits with constant rates $k_+$ and $k_-$; put $K=k_++k_-$. The [probability](../../../../probability.md) density for the first exit to be forward at $t_1$ is $k_+e^{-Kt_1}$. For the very next exit also to be forward at time $t$, multiply by $k_+e^{-K(t-t_1)}$ and integrate over the unobserved first time:

$$
\boxed{\Pr(\hbox{next two exits forward, total time in }dt)
=\int_0^t k_+e^{-Kt_1}k_+e^{-K(t-t_1)}dt_1\,dt
=k_+^2t e^{-Kt}\,dt.}
$$

This density integrates to $(k_+/K)^2$, the [probability](../../../../probability.md) that both directions are forward. Conditional on that event, the normalized total-time density is the [Erlang distribution](../../../../erlang-distribution.md)

$$
\boxed{p(t\mid++)=K^2t e^{-Kt},\qquad t_{\rm mode}=\frac1K\simeq0.010\,\mathrm s.}
$$

Its mean is $2/K$, so the most probable time is not the mean. Since both backward-rate conventions in part (c) have $k_-\ll k_+$, neglecting backwards steps gives the usual approximation $p(t)=k_+^2te^{-k_+t}$ and mode $1/k_+$. If “two forward steps” instead permits intervening backwards events, thinning independent Poisson exits gives that latter rate-$k_+$ distribution directly; it describes a different conditioning. The low barrier noted in part (c) limits the physical accuracy of all these memoryless dwell assumptions.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
