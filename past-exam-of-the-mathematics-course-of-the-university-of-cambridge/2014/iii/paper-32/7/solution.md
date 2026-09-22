<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For mutually exclusive event types, let $T$ be the first event time and $J$ its type. The [cause-specific hazard](../../../../../cause-specific-hazard.md) for cause $j$ is

$$
h_j(t)=\lim_{\Delta\downarrow0}\frac{P(t\le T<t+\Delta,J=j\mid T\ge t)}{\Delta}.
$$

It is a rate conditional on having had no event of any cause. The [cumulative incidence function](../../../../../cumulative-incidence-function.md), also called the [cumulative risk function](../../../../../cumulative-incidence-function.md), is the actual [probability](../../../../../probability.md) $F_j(t)=P(T\le t,J=j)$.

The total [hazard function](../../../../../hazard-function.md) is $h(t)=\sum_kh_k(t)$, giving $S(t)=\exp\{-\int_0^t\sum_kh_k(u)\,du\}$. Surviving every cause to time $u$ and then experiencing cause $j$ gives

$$
\boxed{F_j(t)=\int_0^tS(u)h_j(u)\,du=\int_0^t\exp\left\{-\int_0^u\sum_kh_k(v)\,dv\right\}h_j(u)\,du.}
$$

In [competing risks](../../../../../competing-risks.md), $F_j$ is generally not $1-e^{-\int_0^th_j}$, because competing events remove individuals before they can experience cause $j$. This formula does not require assuming independent latent failure times for the different causes.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
