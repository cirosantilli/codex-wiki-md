<h1 id="32e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\epsilon$ be the group parameter. The [infinitesimal generator of a Lie point symmetry](../../../../../../infinitesimal-generator-of-a-lie-point-symmetry.md)

$$
V=t\partial_t+x\partial_x
$$

has flow equations

$$
\frac{dT}{d\epsilon}=T,
\qquad
\frac{dX}{d\epsilon}=X,
\qquad
\frac{dU}{d\epsilon}=0.
$$

Therefore it generates the scaling group

$$
\boxed{(t,x,u)\longmapsto(e^\epsilon t,e^\epsilon x,u).}
$$

Here $\xi^t=t$, $\xi^x=x$, and $\eta=0$. The total-derivative formulas for the [second prolongation of a Lie point symmetry](../../../../../../second-prolongation-of-a-lie-point-symmetry.md) give

$$
\eta^t=-u_t,
\qquad \eta^x=-u_x,
$$

and

$$
\eta^{tt}=-2u_{tt},
\qquad
\eta^{tx}=-2u_{tx},
\qquad
\eta^{xx}=-2u_{xx}.
$$

Thus

$$
\boxed{
\operatorname{pr}^{(2)}V
=t\partial_t+x\partial_x
-u_t\partial_{u_t}-u_x\partial_{u_x}
-2u_{tt}\partial_{u_{tt}}
-2u_{tx}\partial_{u_{tx}}
-2u_{xx}\partial_{u_{xx}}.}
$$

For the [wave equation](../../../../../../wave-equation-split.md) expression $F=u_{tt}-u_{xx}$,

$$
\operatorname{pr}^{(2)}V(F)=-2F.
$$

It therefore vanishes whenever $F=0$, proving that $V$ generates the [simultaneous spacetime scaling symmetry of the wave equation](../../../../../../simultaneous-spacetime-scaling-symmetry-of-the-wave-equation.md).

The independent invariant of the scaling orbits is the [similarity variable](../../../../../../similarity-variable.md)

$$
z=\frac xt,
$$

while $u$ itself is invariant. Seek a [group-invariant solution](../../../../../../group-invariant-solution.md) $u(t,x)=f(z)$. Direct [partial differentiation](../../../../../../partial-derivative.md) gives

$$
u_{tt}=\frac{z^2f''+2zf'}{t^2},
\qquad
u_{xx}=\frac{f''}{t^2}.
$$

The wave equation reduces to

$$
(z^2-1)f''+2zf'=0
\quad\Longleftrightarrow\quad
\frac d{dz}\left((z^2-1)f'\right)=0.
$$

Hence, on any interval avoiding $z=\pm1$,

$$
\boxed{
u(t,x)=C_0+\frac{C_1}{2}
\log\left|\frac{x-t}{x+t}\right|.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32E](../../32e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
