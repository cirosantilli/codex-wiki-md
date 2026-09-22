<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix an outer radius $R>\rho=|z_0|$. By continuity, reaching zero before radius $R$ requires first reaching every radius $\varepsilon\in(0,\rho)$. The [planar Brownian annulus hitting probability](../../../../../planar-brownian-annulus-hitting-probability.md) from (i) therefore implies

$$
0\leq\mathbb P(\tau_0<\tau_R)
\leq\mathbb P(\tau_\varepsilon<\tau_R)
=\frac{\log(R/\rho)}{\log(R/\varepsilon)}\longrightarrow0
\quad(\varepsilon\downarrow0).
$$

Thus $\mathbb P(\tau_0<\tau_R)=0$ for every fixed $R>\rho$.

On any continuous [sample path](../../../../../sample-path.md) that reaches zero in finite time, the radius has a finite maximum before that time. There is therefore some integer $m>\rho$ for which zero is reached before radius $m$. Consequently

$$
\{\tau_0<\infty\}=\bigcup_{m\in\mathbb N,\,m>\rho}\{\tau_0<\tau_m\}.
$$

Every event on the right has [probability](../../../../../probability.md) zero, so

$$
\boxed{\mathbb P(\tau_0=\infty)=1.}
$$

This proves that [planar Brownian motion avoids a fixed point](../../../../../planar-brownian-motion-avoids-a-fixed-point.md) even though it can reach arbitrarily small positive radii.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
