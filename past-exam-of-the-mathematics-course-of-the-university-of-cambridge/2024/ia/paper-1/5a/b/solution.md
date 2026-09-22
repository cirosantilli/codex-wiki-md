<h1 id="5a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
c=y\cdot z,\qquad p=x\cdot y,\qquad q=x\cdot z.
$$

Since $x,y,z$ are unit [vectors](../../../../../../vector.md),

$$
S=2-p^2-q^2+p+q
=\frac52-\left(p-\frac12\right)^2
-\left(q-\frac12\right)^2.
$$

The [feasible inner products with two unit vectors](../../../../../../feasible-inner-products-with-two-unit-vectors.md) satisfy

$$
\frac{p^2-2cpq+q^2}{1-c^2}\leq1.
$$

The desired pair $p=q=1/2$ is feasible exactly when $c\geq-1/2$. In that case every maximizer has these [inner products](../../../../../../inner-product.md). If $c<-1/2$, symmetry and strict convexity force $p=q$, and the nearest feasible diagonal point is

$$
p=q=\sqrt{\frac{1+c}{2}}.
$$

Using the [vector triple product](../../../../../../vector-triple-product.md),

$$
x\times(y\times z)=y(x\cdot z)-z(x\cdot y)=qy-pz.
$$

Hence

$$
\boxed{
F(y,z)=
\begin{cases}
\dfrac12(y-z),&y\cdot z\geq-\dfrac12,\\[6pt]
\sqrt{\dfrac{1+y\cdot z}{2}}\,(y-z),
&y\cdot z<-\dfrac12.
\end{cases}}
$$

Rotations preserve dot products and cross-product lengths, while $z'=2z$. Thus

$$
S'=5-p^2-4q^2+p+2q
=\frac{11}{2}
-\left(p-\frac12\right)^2
-4\left(q-\frac14\right)^2.
$$

Let

$$
t=\begin{pmatrix}1/2\\1/4\end{pmatrix},
\qquad
K=\begin{pmatrix}1&c\\c&1\end{pmatrix},
\qquad
W=\begin{pmatrix}1&0\\0&4\end{pmatrix}.
$$

The target pair is feasible precisely when

$$
t^TK^{-1}t=\frac{5-4c}{16(1-c^2)}\leq1,
$$

or

$$
\frac{1-3\sqrt5}{8}\leq c\leq
\frac{1+3\sqrt5}{8}.
$$

On this interval,

$$
\boxed{G(y,z)=\frac14y-\frac12z}.
$$

Outside this interval, let $\lambda>0$ be the unique number for which

$$
r=(W+\lambda K^{-1})^{-1}Wt,
\qquad
r^TK^{-1}r=1,
$$

and write $r=(p,q)^T$. These equations give the unique weighted projection of $t$ onto the feasible ellipse, and therefore determine the maximizing [inner products](../../../../../../inner-product.md) solely from $c=y\cdot z$. In the remaining cases,

$$
\boxed{G(y,z)=qy-pz}.
$$

Neither answer depends on $\theta_1$ or $\theta_2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5A](../../5a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
