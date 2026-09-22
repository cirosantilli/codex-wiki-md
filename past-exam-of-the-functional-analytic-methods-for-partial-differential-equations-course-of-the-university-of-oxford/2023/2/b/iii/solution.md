<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First repeat the [Caccioppoli inequality](../../../../../caccioppoli-inequality.md) calculation on two concentric [balls](../../../../../ball-mathematics.md). If $h$ is a [harmonic function](../../../../../harmonic-function.md) on $B_R$, choose a [cutoff function](../../../../../cutoff-function.md) equal to one on $B_r$, supported in $B_R$, and with [gradient](../../../../../gradient.md) bounded by $C/(R-r)$. The argument of (ii), with $A=I$ and $k=0$, gives

$$
\int_{B_r}|\nabla h|^2\,dx\leq\frac{C_*}{(R-r)^2}\int_{B_R}|h|^2\,dx
\qquad(0<r<R\leq1).
$$

Here $C_*$ depends at most on the dimension. When $h$ is only known to be smooth inside $B_R$ and in $L^2(B_R)$, the [weak formulation](../../../../../weak-formulation.md) and all [integrals](../../../../../integral-split.md) involving the [cutoff function](../../../../../cutoff-function.md) are still legitimate, since its [support](../../../../../support.md) is strictly inside $B_R$.

Every classical [partial derivative](../../../../../partial-derivative.md) of the given smooth [harmonic function](../../../../../harmonic-function.md) $u$ is again a [harmonic function](../../../../../harmonic-function.md), since constant-coefficient [partial derivatives](../../../../../partial-derivative.md) commute with the [Laplacian](../../../../../laplacian.md). Choose indices $i_1,\ldots,i_m$ representing the [multi-index](../../../../../multi-index-notation.md) $\alpha$, and define

$$
h_0=u,\qquad h_j=\partial_{i_j}\cdots\partial_{i_1}u,\qquad
R_j=1-\frac{j}{2m}\quad(0\leq j\leq m).
$$

For each $j\geq1$, the preceding [Caccioppoli inequality](../../../../../caccioppoli-inequality.md) yields

$$
\int_{B_{R_j}}|h_j|^2
\leq\int_{B_{R_j}}|\nabla h_{j-1}|^2
\leq C_*(2m)^2\int_{B_{R_{j-1}}}|h_{j-1}|^2.
$$

Starting with $u\in L^2(B_1)$, these estimates also establish the integrability needed at each subsequent step. Iterating $m$ times gives

$$
\boxed{\int_{B_{1/2}}|\partial^\alpha u|^2\,dx
\leq\bigl(4C_*m^2\bigr)^m\int_{B_1}|u|^2\,dx.}
$$

This is the desired [interior derivative estimate for a harmonic function](../../../../../interior-derivative-estimate-for-a-harmonic-function.md), with a constant depending only on $n$ and $m$, uniformly over every [multi-index](../../../../../multi-index-notation.md) of size $m$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
