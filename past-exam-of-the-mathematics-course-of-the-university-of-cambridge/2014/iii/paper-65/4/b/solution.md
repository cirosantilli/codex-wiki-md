<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fidelity norm here is **unsquared**, as in the original PDF. Write $(s)_+=\max(s,0)$, so $h(Gu)=\sum_i((Gu)_i)_+^2$. Introduce $a,q\in\mathbb R^n$ and $t\in\mathbb R$. The [second-order cone reformulation of one-sided quadratic denoising](../../../../../../second-order-cone-reformulation-of-one-sided-quadratic-denoising.md) is

$$
\boxed{\min_{u,a,q,t}\ t+\lambda\sum_iq_i}
$$

subject to the affine cone constraints

$$
(t,u-g)\in\mathcal Q_{n+1},\qquad
\left(\frac{q_i+1}{2},\frac{q_i-1}{2},a_i\right)\in\mathcal Q_3,\qquad
a_i\geq0,\quad a_i-(Gu)_i\geq0\quad(i=1,\ldots,n),
$$

where $\mathcal Q_d=\{(r,z):r\geq\|z\|_2\}$ is the [second-order cone](../../../../../../second-order-cone.md). All coordinates displayed inside the cone memberships are affine in the optimization variables, so stacking them has precisely the form $Ax-b\in K$. The first cone enforces $t\geq\|u-g\|_2$, and each three-dimensional cone enforces $q_i\geq a_i^2$. The two scalar inequalities give $a_i\geq((Gu)_i)_+$.

Every feasible lift therefore has objective at least the original objective. Conversely, for any $u$, choose $a_i=((Gu)_i)_+$, $q_i=a_i^2$ and $t=\|u-g\|_2$ to attain equality. Thus the reformulation is exact. It is a [second-order cone program](../../../../../../second-order-cone-programming.md) over the product $K=\mathcal Q_{n+1}\times\mathcal Q_3^n\times\mathbb R_+^{2n}$, a proper closed self-dual cone. It preserves the asymmetric derivative penalty; replacing it by $\|Gu\|^2$ would change the problem.

The canonical Lorentz-cone barrier is $-\log(r^2-\|z\|^2)$ on $r>\|z\|$, and each orthant coordinate contributes $-\log s$. Their sum, composed with the affine slack map, is

$$
\boxed{\mathcal B(u,a,q,t)=-\log(t^2-\|u-g\|^2)
-\sum_i\log(q_i-a_i^2)-\sum_i\log a_i
-\sum_i\log(a_i-(Gu)_i).}
$$

Its domain explicitly requires $t>\|u-g\|$, $q_i>a_i^2$, $a_i>0$ and $a_i>(Gu)_i$; the positive Lorentz branch must not be inferred merely from positivity of a squared expression. The barrier parameter of the product-cone barrier is $\boxed{\nu=4n+2}$, with two per Lorentz block and one per scalar orthant slack. A strict feasible lift can always be obtained by choosing $a$ above both bounds, $q$ above $a^2$, and $t$ above the fidelity norm.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
