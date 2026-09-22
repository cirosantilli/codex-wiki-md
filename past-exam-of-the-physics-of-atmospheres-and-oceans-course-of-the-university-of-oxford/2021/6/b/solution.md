<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $m=\pi/b$. With $r=0$, [Sverdrup balance](../../../../sverdrup-balance.md) gives

$$
\boxed{v(y)=\frac{F_0}\beta\cos(my).}
$$

At an impermeable eastern wall, $u(L,y)=0$. Continuity implies

$$
u_x=-v_y=\frac{mF_0}\beta\sin(my),\qquad
\boxed{u(x,y)=\frac{mF_0}\beta(x-L)\sin(my).}
$$

Equivalently,

$$
\psi(x,y)=\frac{F_0}\beta(x-L)\cos(my)
$$

satisfies the [impermeability condition](../../../../no-penetration-boundary-condition.md) with the boundary [streamfunction](../../../../stream-function.md) set to zero.

At a second wall $x=0$, this solution has $u(0,y)=-mF_0L\sin(my)/\beta$, generally nonzero. A useful integral proof of the obstruction is

$$
\frac d{dy}\int_0^L v\,dx=-[u(L,y)-u(0,y)]=0
$$

for two impermeable walls, whereas the proposed interior gives $\int_0^L v\,dx=LF_0\cos(my)/\beta$, which varies with $y$. Friction or another departure from the inviscid model is needed for a return flow that closes the circulation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
