<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $(r_0,r_1,r_2)$ be any ordering of the three distinct numbers $0,1,\lambda$. Set $h=r_1-r_0$ and choose $s\ne0$ with $s^2=h^3$. The [projective transformation](../../../../projective-linear-transformation.md)

$$
\begin{pmatrix}X\\Y\\Z\end{pmatrix}
=\begin{pmatrix}
1/h&0&-r_0/h\\
0&1/s&0\\
0&0&1
\end{pmatrix}
\begin{pmatrix}x\\y\\z\end{pmatrix}
$$

has the required matrix form. As $x=hX+r_0Z$ and $y=sY$, substitution gives

$$
Y^2Z=X(X-Z)(X-\widetilde\lambda Z),
\qquad
\boxed{\widetilde\lambda=\frac{r_2-r_0}{r_1-r_0}.}
$$

The choice $s^2=h^3$ is exactly what cancels the coefficient introduced by the change in $x$.

The six orderings give the [Legendre parameter orbit](../../../../legendre-parameter-orbit.md):

$$
\begin{array}{c|c}
(r_0,r_1,r_2)&\widetilde\lambda\\\hline
(0,1,\lambda)&\lambda\\
(1,0,\lambda)&1-\lambda\\
(0,\lambda,1)&1/\lambda\\
(\lambda,0,1)&(\lambda-1)/\lambda\\
(1,\lambda,0)&1/(1-\lambda)\\
(\lambda,1,0)&\lambda/(\lambda-1)
\end{array}
$$

Every entry is different from $0,1$ when $\lambda\ne0,1$.

There are no further possibilities for a matrix of the stated form. Its [determinant](../../../../determinant.md) is $acd$, so $a,c,d$ must be nonzero. On $z=1$ it induces the affine change $u\mapsto(a/d)u+b/d$ and scales $v=y/z$ by $c/d$. It preserves the line $y=0$, whose three intersections with the [plane cubic](../../../../plane-cubic.md) have $u$-coordinates $0,1,\lambda$. Their images must have coordinates $0,1,\widetilde\lambda$. Choosing the two roots sent to $0,1$ determines the affine change and leaves exactly the six orderings above.

For general $\lambda$ the six values are distinct. They coincide in some special cases: $\lambda\in\{-1,2,1/2\}$ gives three values, and $\lambda^2-\lambda+1=0$ gives two. In particular, for the value obtained in part (c), the two possible values are $(1\pm\mathrm i\sqrt3)/2$. This does not contradict the paper's qualification that there are six for general $\lambda$.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the algebraic curves course of the University of Oxford](../../../split.md)
5. [Algebraic curves course of the University of Oxford](../../../../algebraic-curves-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
