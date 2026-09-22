<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the initial-curve parameter $s$ and a characteristic parameter $t$. [Charpit's equations](../../../../../charpit-s-equations.md) are

$$
\boxed{\dot x=F_p,\quad\dot y=F_q,\quad\dot u=pF_p+qF_q,\quad\dot p=-F_x-pF_u,\quad\dot q=-F_y-qF_u.}
$$

At $t=0$ prescribe $x=x_0(s)$, $y=y_0(s)$ and $u=u_0(s)$. The two initial [derivatives](../../../../../derivative.md) $p_0,q_0$ must satisfy

$$
\boxed{F(x_0,y_0,u_0,p_0,q_0)=0,\qquad p_0x_0'+q_0y_0'=u_0'.}
$$

The second equation is the [chain rule](../../../../../chain-rule.md) along the initial curve. For the usual local Cauchy construction also require the [non-characteristic](../../../../../non-characteristic-hypersurface.md) condition $x_0'F_q-y_0'F_p\ne0$. It ensures both local determination of an allowed branch of $p_0,q_0$ and local inversion of the projected characteristic coordinates.

Along a characteristic, the [chain rule](../../../../../chain-rule.md) and the five equations give

$$
\frac{dF}{dt}=F_xF_p+F_yF_q+F_u(pF_p+qF_q)-F_p(F_x+pF_u)-F_q(F_y+qF_u)=0.
$$

Since $F=0$ initially, $\boxed{F\equiv0}$ along each constructed curve. With the contact compatibility $du=p\,dx+q\,dy$ propagated by this system, an invertible characteristic chart reconstructs $p=u_x,q=u_y$ and hence a local [classical solution](../../../../../classical-solution.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
