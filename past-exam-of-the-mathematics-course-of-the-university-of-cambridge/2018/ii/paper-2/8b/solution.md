<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

In Cartesian coordinates the Lagrangian is

$$
\mathcal L=\frac12(\dot x^2+\dot y^2+\dot z^2)+y\dot x.
$$

Introduce a [Lagrange multiplier](../../../../../lagrange-multiplier.md) $\lambda$ for $x^2+y^2+z^2=c^{-2}$. The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) become

$$
\ddot x+\dot y=\lambda x,
\qquad
\ddot y-\dot x=\lambda y,
\qquad
\ddot z=\lambda z,
$$

or

$$
\ddot{\mathbf x}+\dot y\,\mathbf i-\dot x\,\mathbf j
=\lambda\mathbf x.
$$

Differentiating the constraint twice gives

$$
\mathbf x\mathbin\cdot\dot{\mathbf x}=0,
\qquad
\mathbf x\mathbin\cdot\ddot{\mathbf x}=-|\dot{\mathbf x}|^2.
$$

Taking the scalar product of the vector equation with $\mathbf x$ therefore yields

$$
\lambda=c^2\left(-|\dot{\mathbf x}|^2+x\dot y-y\dot x\right).
$$

Substitution gives

$$
\boxed{\ddot{\mathbf x}+\dot y\,\mathbf i-\dot x\,\mathbf j
+c^2\left(|\dot{\mathbf x}|^2+y\dot x-x\dot y\right)\mathbf x=0.}
$$

For $c=0$, the equations have the first integrals

$$
\dot x+y=A,
\qquad
\dot y-x=B,
\qquad
\dot z=C.
$$

Writing $X=x+B$ and $Y=y-A$ gives $\dot X=-Y$ and $\dot Y=X$. Hence every trajectory is

$$
\boxed{x(t)=R\cos(t-t_0)-B,
\qquad
y(t)=R\sin(t-t_0)+A,
\qquad
z(t)=Ct+D.}
$$

These are [helices](../../../../../helical-motion-in-a-uniform-magnetic-field.md) of unit angular frequency about a line parallel to the $z$ axis, including circles when $C=0$ and a straight line when $R=0$.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
