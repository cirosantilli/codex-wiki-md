<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the standard bounded [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) assumption: $\xi\cdot a(y)\xi\ge\alpha|\xi|^2$ for some $\alpha>0$, with bounded periodic coefficients. It holds for the usual finite set of positive-conductivity phases. Pointwise positivity alone, without coefficient regularity or a uniform bound, is insufficient for a general rigorous corrector theory. The calculation below is the requested formal bulk expansion; for nonsymmetric [uniformly elliptic](../../../../../../uniformly-elliptic-operator.md) coefficients the flux derivation still works.

Set $y=x/\epsilon$. In a [two-scale expansion for periodic conductivity](../../../../../../two-scale-expansion-for-periodic-conductivity.md), differentiation becomes

$$
D_i=\partial_{x_i}+\epsilon^{-1}\partial_{y_i}.
$$

The leading, order $\epsilon^{-2}$, equation is

$$
-\partial_{y_i}(a_{ij}\partial_{y_j}u_0)=0.
$$

For fixed $x$, multiply by $u_0$ minus its cell mean and integrate over the periodic cell. Opposite-face terms cancel, giving

$$
0=\int_Y(\nabla_yu_0)\cdot a(y)\nabla_yu_0\,dy
\ge\alpha\int_Y|\nabla_yu_0|^2\,dy.
$$

Hence **$u_0$ is independent of $y$**.

The order $\epsilon^{-1}$ equation is now

$$
\partial_{y_i}\left[a_{ij}\bigl(\partial_{x_j}u_0+\partial_{y_j}u_1\bigr)\right]=0.
$$

For each coordinate direction, choose a periodic zero-mean corrector $w_j$ satisfying the [periodic conductivity cell problem](../../../../../../periodic-conductivity-cell-problem.md)

$$
\boxed{\partial_{y_i}\left(a_{ik}\partial_{y_k}w_j\right)=-\partial_{y_i}a_{ij}.}
$$

The right side has zero cell mean. In weak form,

$$
\int_Y\nabla\phi\cdot a\nabla w_j\,dy
=-\int_Y\nabla\phi\cdot ae_j\,dy
$$

for every periodic test function $\phi$. On the space of zero-mean [periodic functions](../../../../../../periodic-function.md), the [Poincaré inequality](../../../../../../poincare-inequality.md) and [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) give coercivity, so the corrector exists and is unique by the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md). Discontinuous phase coefficients are handled by this [weak formulation](../../../../../../weak-formulation.md).

The order $\epsilon^{-1}$ solution is

$$
u_1(x,y)=w_j(y)\partial_{x_j}u_0(x)+\bar u_1(x),
$$

where the last term is independent of $y$ and does not affect leading flux. Thus the leading microscopic flux is

$$
h_i^{(0)}=a_{ik}(y)\left(\delta_{kj}+\partial_{y_k}w_j\right)\partial_{x_j}u_0.
$$

At order one the equation reads

$$
-\partial_{x_i}h_i^{(0)}
-\partial_{y_i}\left[a_{ij}\bigl(\partial_{x_j}u_1+\partial_{y_j}u_2\bigr)\right]=f.
$$

Average over $Y$. The second term integrates to zero by periodicity, and $|Y|=1$. Therefore

$$
\boxed{
a_{ij}^*=\int_Y\left(a_{ij}+a_{ik}\partial_{y_k}w_j\right)\,dy,\qquad
-\partial_{x_i}(a_{ij}^*\partial_{x_j}u_0)=f.
}
$$

The effective [tensor](../../../../../../tensor.md) is constant, so the last equation is exactly $-a_{ij}^*\partial_{x_i}\partial_{x_j}u_0=f$. The macroscopic [boundary condition](../../../../../../boundary-condition.md) is $u_0=0$ on $\partial\Omega$. Higher bulk correctors usually do not individually vanish on the physical boundary; a [boundary corrector in periodic homogenization](../../../../../../boundary-corrector-in-periodic-homogenization.md) handles this without changing the leading homogenized equation.

For symmetric $a$, a useful check on the [effective conductivity](../../../../../../effective-conductivity.md) is

$$
a_{ij}^*=\int_Y(e_i+\nabla w_i)\cdot a(e_j+\nabla w_j)\,dy.
$$

The extra term involving $\nabla w_i$ vanishes by the weak cell equation. This formula proves [symmetry](../../../../../../symmetry-physics.md). With $w_\xi=\xi_jw_j$, it also gives $\xi\cdot a^*\xi\ge\alpha\int_Y|\xi+\nabla w_\xi|^2\ge\alpha|\xi|^2$, confirming that the effective [tensor](../../../../../../tensor.md) is [positive-definite](../../../../../../positive-definite-bilinear-form.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
