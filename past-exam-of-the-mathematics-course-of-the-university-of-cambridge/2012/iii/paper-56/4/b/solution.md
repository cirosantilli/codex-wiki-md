<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The displayed $e^a$ are one-forms, so they form an [orthonormal coframe](../../../../../../orthonormal-coframe-in-spacetime.md), dual to the [orthonormal frame](../../../../../../orthonormal-frame-in-spacetime.md) $E_0=A^{-1}\partial_t$, $E_1=A^{-1}\partial_x$, $E_2=A^{-1}\partial_y$, $E_3=\partial_z$. Use $\eta_{ab}=\operatorname{diag}(-1,1,1,1)$ and abbreviate

$$
a=\frac{A'}A,\qquad q=\frac{A''}A=a'+a^2.
$$

For $i=0,1,2$, $de^i=a e^3\wedge e^i$, while $de^3=0$. The [Levi-Civita connection](../../../../../../levi-civita-connection.md) is fixed by [Cartan's first structure equation](../../../../../../cartan-s-first-structure-equation.md) together with [Lorentzian connection-form antisymmetry](../../../../../../lorentzian-connection-form-antisymmetry.md), $\omega_{ab}=-\omega_{ba}$, where $\omega_{ab}=\eta_{ac}\omega^c{}_b$. Its nonzero [connection 1-forms](../../../../../../connection-1-form-split.md) are

$$
\boxed{\omega^0{}_3=a e^0,\quad\omega^1{}_3=a e^1,\quad\omega^2{}_3=a e^2,\quad\omega^3{}_0=a e^0,\quad\omega^3{}_1=-a e^1,\quad\omega^3{}_2=-a e^2.}
$$

In particular, the time-index pair has the same sign with one index raised; incorrectly imposing $\omega^a{}_b=-\omega^b{}_a$ would lose the Lorentzian sign. All diagonal and all other entries vanish.

Apply [Cartan's second structure equation](../../../../../../cartan-s-second-structure-equation.md). For $i=0,1,2$,

$$
\Theta^i{}_3=d(a e^i)=(a'+a^2)e^3\wedge e^i=-q e^i\wedge e^3.
$$

For distinct $i,j$ in $\{0,1,2\}$, putting $s_0=-1$ and $s_1=s_2=1$ gives $\Theta^i{}_j=\omega^i{}_3\wedge\omega^3{}_j=-s_j a^2e^i\wedge e^j$. Thus a complete independent set of [curvature 2-forms](../../../../../../curvature-2-form.md) is

$$
\boxed{\begin{aligned}\Theta^0{}_1&=-a^2e^0\wedge e^1,&\Theta^0{}_2&=-a^2e^0\wedge e^2,&\Theta^1{}_2&=-a^2e^1\wedge e^2,\\\Theta^0{}_3&=-q e^0\wedge e^3,&\Theta^1{}_3&=-q e^1\wedge e^3,&\Theta^2{}_3&=-q e^2\wedge e^3.\end{aligned}}
$$

All diagonal entries vanish. The remaining entries follow from $\Theta_{ab}=-\Theta_{ba}$: $\Theta^j{}_i=-s_is_j\Theta^i{}_j$ for $i,j\le2$, and $\Theta^3{}_i=-s_i\Theta^i{}_3$. These relations and the displayed six entries specify all sixteen [curvature 2-forms](../../../../../../curvature-2-form.md). This computation is [Cartan curvature of a planar warped spacetime](../../../../../../cartan-curvature-of-a-planar-warped-spacetime.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
