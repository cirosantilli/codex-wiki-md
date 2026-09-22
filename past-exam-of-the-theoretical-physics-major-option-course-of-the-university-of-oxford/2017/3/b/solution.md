<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiply the [master equation](../../../../master-equation.md) by $z^n$ and sum over $n$. Shifting indices produces

$$
\boxed{\partial_tF=(z-1)\sum_nq_nz^nP_n+(z^{-1}-1)\sum_nr_nz^nP_n.}
$$

The apparent negative power causes no problem at $z=0$ when $r_0=0$. Let $D=z\partial_z$, so $Dz^n=nz^n$. If the rates are polynomials in $n$, replace their arguments by $D$ to obtain a finite-order [partial differential equation](../../../../partial-differential-equation-split.md):

$$
\boxed{\partial_tF=\bigl[(z-1)q(D)+(z^{-1}-1)r(D)\bigr]F.}
$$

For arbitrary rates the weighted sums still give an exact generating-function evolution, but need not reduce to a finite-order differential operator. The [probability generating function](../../../../probability-generating-function.md) obeys

$$
\boxed{F(1,t)=1,}
$$

which is the normalization condition. The evolution has $\partial_tF(1,t)=0$ when the rate sums converge, so an initially normalized distribution stays normalized. Its derivatives at $z=1$ also give the factorial [moments](../../../../moment.md), and expansion around $z=0$ recovers individual [probabilities](../../../../probability.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
