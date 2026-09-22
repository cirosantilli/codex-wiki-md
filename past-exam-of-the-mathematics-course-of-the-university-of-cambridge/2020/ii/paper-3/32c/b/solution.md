<h1 id="32c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The transformations

$$
g^s:(X,T,u)\longmapsto(e^sX,e^{-s}T,u)
$$

form a [one-parameter group](../../../../../../one-parameter-subgroup.md) with infinitesimal generator

$$
V=X\partial_X-T\partial_T.
$$

Under this scaling, $\partial_X$ has weight $-1$ and $\partial_T$ has weight $1$, so $u_{XT}$ has weight zero, as does $\sin u$. Thus $u_{XT}=\sin u$ is invariant and $g^s$ is a [Scaling symmetry of the sine-Gordon equation](../../../../../../scaling-symmetry-of-the-sine-gordon-equation.md).

The product

$$
z=XT
$$

is invariant under the group. A [group-invariant solution](../../../../../../group-invariant-solution.md) therefore has the form $u(X,T)=F(z)$. Since

$$
u_X=TF'(z),
\qquad
u_{XT}=F'(z)+zF''(z),
$$

the [Sine-Gordon equation](../../../../../../sine-gordon-equation.md) reduces to

$$
zF''+F'=\sin F.
$$

Now put $w=e^{iF}$. Then

$$
F'=-i\frac{w'}w,
\qquad
F''=-i\left(\frac{w''}w-\frac{(w')^2}{w^2}\right),
\qquad
\sin F=\frac{w-w^{-1}}{2i}.
$$

Substitution and multiplication by $iw$ give

$$
zw''-z\frac{(w')^2}{w}+w'
=\frac{w^2-1}{2}.
$$

Hence

$$
\boxed{
w''=\frac{(w')^2}{w}-\frac{w'}z+\frac{w^2-1}{2z}}.
$$

This is the [Painlevé III equation](../../../../../../painleve-iii-equation.md) with parameters $(\alpha,\beta,\gamma,\delta)=(1/2,-1/2,0,0)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [32C](../../32c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
