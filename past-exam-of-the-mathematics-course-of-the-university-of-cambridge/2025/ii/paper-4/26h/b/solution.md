<h1 id="26h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The map $(x,u)\mapsto(x,y)=(x,xu)$ has inverse $u=y/x$ and Jacobian magnitude $1/x$. Hence the density of $(X,Y)$ is

$$
\boxed{f_{X,Y}(x,y)=\frac{g(x)}x
\mathbf 1_{\{x>0,\,0\leq y\leq x\}}}.
$$

For $(y,z)=(xu,x(1-u))$, the inverse is

$$
x=y+z,
\qquad
u=\frac y{y+z},
$$

and the Jacobian magnitude of $(y,z)\mapsto(x,u)$ is $1/(y+z)$. Thus the [uniform split of a random total](../../../../../../uniform-split-of-a-random-total.md) has joint density

$$
\boxed{f_{Y,Z}(y,z)=\frac{g(y+z)}{y+z}
\mathbf 1_{\{y,z\geq0\}}}.
$$

Integrating out the other piece yields

$$
\boxed{f_Y(y)=\int_0^\infty\frac{g(y+z)}{y+z}\,dz=h(y)},
\qquad y\geq0.
$$

The transformation $U\mapsto1-U$ preserves the uniform law, so $Z$ has the same density:

$$
\boxed{f_Z(z)=h(z)},
\qquad z\geq0.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26H](../../26h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
