<h1 id="30e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The first-order [Cauchy-Kovalevskaya theorem](../../../../../../cauchy-kovalevskaya-theorem.md) says that an analytic PDE system solved for the [derivative](../../../../../../derivative.md) normal to an analytic noncharacteristic initial hypersurface, with analytic initial data, has a unique local analytic solution near each point of that hypersurface. The general theorem likewise applies to higher-order equations solved for the highest normal [derivative](../../../../../../derivative.md) with analytic data for the lower normal [derivatives](../../../../../../derivative.md).

Here the characteristic vector is $(x,y,a)$ and the normal to $z=0$ is $(0,0,1)$. Its normal component is $a$, so the theorem applies precisely when **$a\ne0$**. The [method of characteristics](../../../../../../method-of-characteristics.md) gives $\dot x=x$, $\dot y=y$, $\dot z=a$, $\dot u=u$. Starting from $(\xi,\eta,0)$ at parameter $s=0$ gives $x=\xi e^s$, $y=\eta e^s$, $z=as$, $u=e^sf(\xi,\eta)$. Eliminating $s=z/a$ yields

$$
\boxed{u(x,y,z)=e^{z/a}f(xe^{-z/a},ye^{-z/a})}.
$$

This is locally defined wherever the arguments remain in the analytic domain of $f$, and verifies both PDE and initial data.

As $a\to0$, the normal component vanishes and the characteristic curves become tangent to the initial plane. The crossing parameter $s=z/a$ and slopes $dx/dz=x/a$, $dy/dz=y/a$ become singular. At $a=0$, arbitrary analytic data are not admissible: already on the plane they must obey $xf_x+yf_y=f$. Even compatible data do not determine [derivatives](../../../../../../derivative.md) normal to the plane. This is failure of the noncharacteristic condition, not a failure of the analytic theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30E](../../30e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
