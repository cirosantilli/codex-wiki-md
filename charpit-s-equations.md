<h1 id="charpit-s-equations">Charpit's equations</h1>

↑ **Parent:** [Method of characteristics](method-of-characteristics.md)

For a first-order nonlinear [partial differential equation](partial-differential-equation-split.md) $F(x,y,u,p,q)=0$, with $p=u_x,q=u_y$, Charpit's equations extend the [method of characteristics](method-of-characteristics.md) to the five-dimensional space of position, value and gradient:

$$
\dot x=F_p,\quad\dot y=F_q,\quad\dot u=pF_p+qF_q,\quad\dot p=-F_x-pF_u,\quad\dot q=-F_y-qF_u.
$$

The chain rule gives $dF/dt=0$ by direct cancellation, so a trajectory starting on $F=0$ remains there. Initial data $u_0(s)$ on $(x_0(s),y_0(s))$ require both $F(x_0,y_0,u_0,p_0,q_0)=0$ and $p_0x_0'+q_0y_0'=u_0'$. The [non-characteristic](non-characteristic-hypersurface.md) condition is $x_0'F_q-y_0'F_p\ne0$. It makes the projection onto $(x,y)$ locally invertible. Compatible initial contact data then propagate as $du=p\,dx+q\,dy$, reconstructing a classical solution. Multiple permitted initial normal derivatives can give different local branches; loss of the projection [Jacobian determinant](jacobian-determinant.md) marks a [characteristic caustic](characteristic-caustic.md).

**Table of contents**

- [Fold caustic for a cubic Charpit equation](fold-caustic-for-a-cubic-charpit-equation.md)

## ↑ Ancestors (8)

1. [Method of characteristics](method-of-characteristics.md)
2. [Characteristic curve](characteristic-curve.md)
3. [Transport equation](transport-equation-split.md)
4. [Partial differential equation](partial-differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Solution](past-exam-of-the-differential-equations-and-applications-course-of-the-university-of-oxford/2007/b/5/solution.md)
- [Solution](past-exam-of-the-differential-equations-and-applications-course-of-the-university-of-oxford/2008/b/5/solution.md)
- [Solution](past-exam-of-the-differential-equations-and-applications-course-of-the-university-of-oxford/2009/b/4/solution.md)
- [Solution](past-exam-of-the-differential-equations-and-applications-course-of-the-university-of-oxford/2010/b/4/a/solution.md)
- [Solution](past-exam-of-the-differential-equations-and-applications-course-of-the-university-of-oxford/2010/b/4/b/solution.md)
- [Square-root reduction of a quadratic eikonal equation](square-root-reduction-of-a-quadratic-eikonal-equation.md)
