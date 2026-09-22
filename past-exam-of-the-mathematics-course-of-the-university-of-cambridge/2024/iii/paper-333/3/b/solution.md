<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate horizontal momentum with respect to $z$ and vertical momentum with respect to $x$. When the two equations are subtracted, the terms proportional to $\overline u_z(u'_x+w'_z)$ vanish by [incompressible flow](../../../../../../incompressible-flow.md). The pressure derivatives also cancel, leaving

$$
\boxed{
D_t(u'_z-w'_x)+\overline u_{zz}w'+\sigma'_x=0}.
$$

Differentiate this equation with respect to $x$. Since continuity gives

$$
(u'_z-w'_x)_x
=-(w'_{xx}+w'_{zz}),
$$

one obtains

$$
-D_t\nabla^2w'
+\overline u_{zz}w'_x+\sigma'_{xx}=0.
$$

Apply $D_t$ and use the buoyancy equation $D_t\sigma'=-N^2w'$. Multiplication by $-1$ then gives

$$
\boxed{
D_t^2(w'_{xx}+w'_{zz})
-\overline u_{zz}D_tw'_x
+N^2w'_{xx}=0}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
