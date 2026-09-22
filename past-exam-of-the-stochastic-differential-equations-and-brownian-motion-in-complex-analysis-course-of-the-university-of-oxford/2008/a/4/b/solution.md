<h1 id="a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $s<t<1$, [independence](../../../../../independent-random-variables.md) and the Gaussian [Brownian transition density](../../../../../brownian-transition-density.md) yield the [Chapman-Kolmogorov equation](../../../../../chapman-kolmogorov-equation.md)

$$
\mathbb E[p(1-t,B_t,y)\mid\mathcal F_s]
=\int_{\mathbb R}p(t-s,B_s,z)p(1-t,z,y)\,dz
=p(1-s,B_s,y).
$$

The numerator is positive and its expectation is $p(1,0,y)$, so

$$
\boxed{M_0=1,\quad\mathbb EM_t=1,\quad
\mathbb E(M_t\mid\mathcal F_s)=M_s.}
$$

These statements hold for every $t<1$, in particular on the specified closed interval $[0,T]$.

The function $h(t,z)=p(1-t,z,y)$ solves the [backward heat equation](../../../../../backward-heat-equation.md) $h_t+\tfrac12h_{zz}=0$. [Itô's formula](../../../../../ito-s-lemma.md) therefore gives

$$
dM_t=M_t\theta_t\,dB_t,\qquad
\theta_t=\frac{\partial}{\partial x}\log p(1-t,B_t,y)
=\frac{y-B_t}{1-t}.
$$

On each interval ending before one this adapted continuous integrand is locally square integrable. Thus

$$
\boxed{N_t=\int_0^t\frac{y-B_s}{1-s}\,dB_s,\qquad
\langle N\rangle_t=\int_0^t\frac{(y-B_s)^2}{(1-s)^2}\,ds}
$$

gives $M_t=\exp(N_t-\langle N\rangle_t/2)$. This also follows by applying [Itô's formula](../../../../../ito-s-lemma.md) to $\log M_t$. The source's notation $t\geq0$ for this density process is restricted by its defining formula to $t<1$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
