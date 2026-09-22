<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the fine [matrix](../../../../../matrix.md) $A_h$ and right-hand side from part (b), with diagonal $D_h$. Starting from an iterate $v$, take $\nu$ [weighted Jacobi](../../../../../weighted-jacobi-method.md) smoothing steps

$$
v\leftarrow v+\omega D_h^{-1}(b_h-A_hv),\qquad0<\omega<1.
$$

Form the residual $r_h=b_h-A_hv$. For coarse interior indices $j=1,\ldots,m/2-1$, use [full-weighting restriction](../../../../../full-weighting-restriction.md)

$$
(Rr_h)_j=\tfrac14(r_{2j-1}+2r_{2j}+r_{2j+1}).
$$

The [prolongation operator](../../../../../prolongation-operator.md) [matrix](../../../../../matrix.md) $P$ is linear interpolation of a coarse correction: $(Pe)_{2j}=e_j$ and $(Pe)_{2j+1}=(e_j+e_{j+1})/2$, with zero endpoint corrections. Thus $R=P^T/2$. Choose the [Galerkin coarse-grid operator](../../../../../galerkin-coarse-grid-operator.md) $A_c=RA_hP$, solve $A_ce_c=Rr_h$ exactly, and correct $v\leftarrow v+Pe_c$. The entries of $A_h$, $R$ and $P$ above specify every [matrix](../../../../../matrix.md) in the cycle. A rediscretized coarse operator is another standard choice if used consistently.

For a nonsingular coarse operator, the fine-grid [iteration matrix](../../../../../iteration-matrix.md) of this pre-smoothed two-grid cycle is

$$
\boxed{E_{\rm TG}=(I-PA_c^{-1}RA_h)(I-\omega D_h^{-1}A_h)^\nu.}
$$

The purpose of under-relaxation is to damp fine-grid oscillations, leaving smoother error for coarse-grid correction. For the diffusion-dominated one-dimensional operator, $\omega=2/3$ is the usual effective choice; the high-frequency symbol $1-\omega(1-\cos\xi)$ then has modulus at most $1/3$ for $\pi/2\leq|\xi|\leq\pi$. Coefficients and convection can change the best parameter, so this is a motivated choice rather than a universal optimum. Under the diagonal-dominance condition, the unweighted Jacobi [matrix](../../../../../matrix.md) already has [norm](../../../../../norm.md) less than one in the [maximum norm](../../../../../supremum-norm.md), and its [convex combination](../../../../../convex-combination.md) with the identity remains convergent for $0<\omega<1$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
