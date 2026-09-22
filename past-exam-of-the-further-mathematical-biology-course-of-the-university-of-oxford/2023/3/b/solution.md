<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $K$ as the population scale, $N_0$ as the [nutrient](../../../../nutrient.md) [concentration](../../../../concentration.md) scale, $r^{-1}$ as the time scale, and $L$ as the length scale. The [nondimensionalization](../../../../nondimensionalization.md) is

$$
\boxed{B=Kb,\qquad N=N_0n,\qquad T=t/r,\qquad X=Lx.}
$$

For example, the [chemotaxis](../../../../chemotaxis.md) term becomes

$$
-\chi_B\partial_X\left(\frac{B}{(N_0+N)^2}N_X\right)
=-\frac{\chi_BK}{N_0L^2}\partial_x\left(\frac b{(1+n)^2}n_x\right).
$$

Dividing the population equation by $rK$ and the [nutrient](../../../../nutrient.md) equation by $rN_0$ gives the requested system with the following six [dimensionless quantities](../../../../dimensionless-quantity.md):

$$
\boxed{d_b=\frac{D_B}{rL^2},\qquad d_n=\frac{D_N}{rL^2},\qquad
\chi_b=\frac{\chi_B}{rL^2N_0},\qquad
\lambda=\frac a{rN_0},\qquad b_0=\frac{B_0}{K},\qquad \mu=\frac{dK}{r}.}
$$

The rescaled domain is $0<x<1$, $t>0$. Its [boundary conditions](../../../../boundary-condition.md) and [initial conditions](../../../../initial-condition.md) are

$$
\boxed{b_x(0,t)=b_x(1,t)=n_x(0,t)=n_x(1,t)=0,}
$$



$$
\boxed{b(x,0)=\frac{B_{\mathrm{initial}}(Lx)}K,\qquad
n(x,0)=\frac{N_{\mathrm{initial}}(Lx)}{N_0},\qquad 0\le x\le1.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further mathematical biology course of the University of Oxford](../../../split.md)
5. [Further mathematical biology course of the University of Oxford](../../../../further-mathematical-biology-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
