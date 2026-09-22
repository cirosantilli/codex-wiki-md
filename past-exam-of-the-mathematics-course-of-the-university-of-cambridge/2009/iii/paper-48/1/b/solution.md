<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $I_0=\sqrt{2\pi/m^2}$ and assume $m^2>0$. The normalized free [Gaussian integral](../../../../../../gaussian-integral.md) has covariance $\Delta=1/m^2$. Expanding the interaction exponential and using [Wick's theorem](../../../../../../wick-s-theorem.md) gives the [Feynman rules](../../../../../../feynman-rule.md): a quartic vertex contributes $-\lambda$, each internal [propagator](../../../../../../propagator.md) contributes $\Delta$, and each [vacuum diagram](../../../../../../vacuum-feynman-diagram.md) is divided by its [Feynman-diagram symmetry factor](../../../../../../feynman-diagram-symmetry-factor.md). Multiply the resulting sum by $I_0$. Because we are expanding $I$, rather than $\log I$, disconnected [vacuum diagrams](../../../../../../vacuum-feynman-diagram.md) must also be included.

At order $\lambda^2$ there are two quartic vertices and four internal [propagators](../../../../../../propagator.md). Let $r$ be the number of edges joining the two vertices. The remaining half-edges must pair at their own vertex, so $r$ is even. The possibilities $r=0,2,4$ exhaust the [vacuum diagrams](../../../../../../vacuum-feynman-diagram.md):

<a id="1/b/image-all-three-second-order-quartic-vacuum-diagrams-and-their-symmetry-factors"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-48-vacuum-diagrams.png)

**[Figure 1](#1/b/image-all-three-second-order-quartic-vacuum-diagrams-and-their-symmetry-factors). All three second-order quartic vacuum diagrams and their symmetry factors**.

For $r=0$, each vertex has three possible pairings, giving $N_0=9$ [Wick contractions](../../../../../../wick-contraction.md). For $r=2$, choose the two half-edges at each vertex, then pair the chosen half-edges across the vertices: $N_2=\binom42^2 2!=72$. The remaining two half-edges at each vertex form a self-loop. For $r=4$, all half-edges pair across the vertices, giving $N_4=4!=24$. The common denominator from the expansion is $2!(4!)^2=1152$, so the [Feynman-diagram symmetry factors](../../../../../../feynman-diagram-symmetry-factor.md) are

$$
S_0=\frac{1152}{9}=128,\qquad S_2=\frac{1152}{72}=16,\qquad S_4=\frac{1152}{24}=48.
$$

Each [vacuum diagram](../../../../../../vacuum-feynman-diagram.md) has the same factor $I_0\lambda^2\Delta^4$ before division by its [Feynman-diagram symmetry factor](../../../../../../feynman-diagram-symmetry-factor.md). Consequently the **coefficient of $\lambda^2$** is

$$
\boxed{\frac{I_0}{m^8}\left(\frac1{128}+\frac1{16}+\frac1{48}\right)=\frac{35}{384m^8}\sqrt{\frac{2\pi}{m^2}}.}
$$

As an independent check, the eighth moment obtained from the [Gaussian moment pairing theorem](../../../../../../isserlis-s-theorem.md) is $\langle x^8\rangle_0=7!!/m^8=105/m^8$, and $105/[2!(4!)^2]=35/384$. The first terms of the [zero-dimensional quartic perturbation series](../../../../../../zero-dimensional-quartic-perturbation-series.md) are therefore

$$
\frac{I}{I_0}=1-\frac{\lambda}{8m^4}+\frac{35\lambda^2}{384m^8}+O(\lambda^3).
$$

Strictly, the printed phrase “Taylor expansion” means a formal expansion or a right-sided [asymptotic expansion](../../../../../../asymptotic-expansion.md). The general coefficient has absolute successive ratio $(4v+3)(4v+1)/[24(v+1)m^4]\to\infty$, so the [power series](../../../../../../power-series.md) has zero radius of convergence. Nevertheless, for $\lambda\geq0$ the remainder after any fixed truncation of $e^{-\lambda x^4/4!}$ is bounded by the next absolute term, and its [Gaussian integral](../../../../../../gaussian-integral.md) is finite. This proves the displayed [asymptotic expansion](../../../../../../asymptotic-expansion.md) as $\lambda\downarrow0$. For negative real $\lambda$ the defining integral diverges.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
