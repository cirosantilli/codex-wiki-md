<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md) are

$$
\boxed{Hx=c,\qquad H=G^TG,\quad c=G^Tb}.
$$

The [full column rank](../../../../../full-column-rank.md) of $G$ gives $z^THz=\|Gz\|_2^2>0$ for nonzero $z$, so $H$ is a [symmetric positive-definite matrix](../../../../../symmetric-positive-definite-matrix.md). Apply the [Conjugate gradient method](../../../../../conjugate-gradient-method.md) to this [linear system](../../../../../system-of-linear-equations.md). To verify that its solution is the desired one, let $x_*$ solve the displayed equations. Then $G^T(Gx_*-b)=0$, and for any $x$ the [Pythagorean identity](../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|Gx-b\|_2^2=\|Gx_*-b\|_2^2+\|G(x-x_*)\|_2^2.
$$

Thus $x_*$ is the unique minimizer of the [linear least-squares problem](../../../../../linear-least-squares-problem.md).

One can apply $H$ without forming the [Gram matrix](../../../../../gram-matrix.md): compute $Hp=G^T(Gp)$. More explicitly, initialize $x_0$, $r_0=c-Hx_0$, $p_0=r_0$; until the [linear-system residual](../../../../../linear-system-residual.md) vanishes, use the [Conjugate gradient method](../../../../../conjugate-gradient-method.md) recurrence

$$
\alpha_j=\frac{r_j^Tr_j}{p_j^THp_j},\quad
x_{j+1}=x_j+\alpha_jp_j,\quad
r_{j+1}=r_j-\alpha_jHp_j,
$$



$$
\beta_j=\frac{r_{j+1}^Tr_{j+1}}{r_j^Tr_j},\qquad
p_{j+1}=r_{j+1}+\beta_jp_j.
$$

Each dense application of $H$ this way costs $O(mn)$ operations. The [condition number](../../../../../condition-number.md) satisfies $\kappa_2(H)=\kappa_2(G)^2$, where $\kappa_2(G)=\sigma_{\max}(G)/\sigma_{\min}(G)$; this is the conditioning cost of the [least-squares normal equations](../../../../../normal-equations-for-linear-least-squares.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
