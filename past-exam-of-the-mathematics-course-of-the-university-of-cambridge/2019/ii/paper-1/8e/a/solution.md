<h1 id="8e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
\xi_i(t)=\left.\frac{\partial Q_i(s,t)}{\partial s}\right|_{s=0}
$$

be the infinitesimal generator of the continuous symmetry, and let

$$
p_i=\frac{\partial L}{\partial\dot q_i}
$$

be the [canonical momentum](../../../../../../canonical-momentum.md). [Noether theorem](../../../../../../noether-theorem.md) states that along every trajectory satisfying the [Euler-Lagrange equations](../../../../../../euler-lagrange-equation.md),

$$
\boxed{J=\sum_{i=1}^np_i\xi_i}
$$

is conserved.

Indeed, differentiate the invariance of $L$ with respect to $s$ at zero:

$$
0=\sum_i\left(
\frac{\partial L}{\partial q_i}\xi_i
+\frac{\partial L}{\partial\dot q_i}\dot\xi_i
\right).
$$

On an Euler-Lagrange trajectory, $\partial L/\partial q_i=d p_i/dt$, so

$$
0=\sum_i(\dot p_i\xi_i+p_i\dot\xi_i)
=\frac d{dt}\sum_i p_i\xi_i.
$$

This proves the [Noether conserved quantity for a mechanical point symmetry](../../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8E](../../8e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
