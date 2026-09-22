<h1 id="29d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A homogeneous linear differential operator satisfies $L(e^\varepsilon u)=e^\varepsilon L(u)$, so the scaling $x\mapsto x$, $u\mapsto e^\varepsilon u$ preserves every homogeneous linear equation. Its infinitesimal generator is **$V=u\partial_u$**.

On a patch with $u\ne0$, take $s=\log|u|$, $t=x$. Then $V(s)=1$, $V(t)=0$. Set $w=ds/dt=u'/u$. Since $u''/u=w'+w^2$, division by $u$ reduces the second-order equation to the [Riccati equation](../../../../../../riccati-equation.md)

$$
\boxed{\frac{dw}{dt}+w^2+p(t)w+q(t)=0.}
$$

Recover a nonzero solution by $u=C\exp(\int w\,dt)$, allowing the sign in $C$. The zero solution is separate, and intervals containing zeros of other solutions require separate coordinate patches. The order reduction occurs because the transformed equation depends on $s'$ but not on $s$ itself.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29D](../../29d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
