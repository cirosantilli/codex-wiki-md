<h1 id="28j/solution">Solution</h1>

↑ **Parent:** [28J](../28j.md)

An [Inhomogeneous Poisson process](../../../../../inhomogeneous-poisson-process.md) with intensity $\lambda$ is a counting process with $N_0=0$, independent increments, and

$$
N_t-N_s\sim\operatorname{Poisson}(\Lambda(t)-\Lambda(s)),
\qquad
\Lambda(t)=\int_0^t\lambda(u)\,du.
$$

The continuity and positivity of $\lambda$ make $\Lambda$ strictly increasing.

For $M_t=N_{g(t)}$ and $0\leq s<t$,

$$
M_t-M_s=N_{g(t)}-N_{g(s)}
$$

has a Poisson distribution with mean

$$
\Lambda(g(t))-\Lambda(g(s))=t-s.
$$

Disjoint increments remain independent, so $M$ is a homogeneous rate-one [Poisson process](../../../../../poisson-process.md). Taking $g=\Lambda^{-1}$ gives $N_t=M_{\Lambda(t)}$, and hence

$$
\boxed{\ N_t\sim\operatorname{Poisson}(\Lambda(t)).\ }
$$

This is the [time change of an inhomogeneous Poisson process](../../../../../time-change-of-an-inhomogeneous-poisson-process.md).

For the bicycle model, let an arrival occur at time $s\leq t$ and have velocity $V$. At time $t$ its position is $V(t-s)$, so it lies in the first $x$ miles exactly when

$$
V(t-s)\leq x.
$$

Conditional on its arrival time, independently marking the bicycle by whether this event occurs is [Poisson thinning](../../../../../poisson-thinning.md). Therefore the desired count is Poisson with mean

$$
\begin{aligned}
\lambda\int_0^t\mathbb P(V(t-s)\leq x)\,ds
&=\lambda\mathbb E\int_0^t\mathbf1_{\{Vu\leq x\}}\,du\\
&=\lambda\mathbb E\left[\min\left(t,\frac{x}{V}\right)\right]\\
&=\lambda\mathbb E\left[V^{-1}\min\{x,Vt\}\right].
\end{aligned}
$$

Thus

$$
\boxed{\ \#\{\text{bicycles in the first }x\text{ miles at time }t\}
\sim\operatorname{Poisson}\!\left(\lambda\mathbb E[V^{-1}\min\{x,Vt\}]\right).\ }
$$

## ↑ Ancestors (10)

1. [28J](../28j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
