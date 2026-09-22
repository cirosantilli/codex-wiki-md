<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\pi,\pi'$ be the $p$-power [Frobenius isogenies](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) of $E,E'$. Since $\psi$ is defined over $\mathbb F_p$, it commutes with Frobenius:

$$
\psi\pi=\pi'\psi,\qquad\psi(1-\pi)=(1-\pi')\psi.
$$

Taking degrees, using multiplicativity and cancelling the nonzero [degree of an isogeny](../../../../../../degree-of-an-isogeny.md) $\deg\psi$, gives

$$
\deg(1-\pi)=\deg(1-\pi').
$$

Both differences are separable, so the preceding proof identifies their degrees with rational point counts. Therefore

$$
\boxed{\#E(\mathbb F_p)=\#E'(\mathbb F_p).}
$$

[Isogenous elliptic curves can have different rational point groups](../../../../../../isogenous-elliptic-curves-can-have-different-rational-point-groups.md). Here is an explicit example. Over $\mathbb F_7$, take

$$
E:y^2=x^3-x,\qquad E':Y^2=X^3+4X.
$$

The map

$$
\psi(x,y)=\left(x-\frac1x,\ y\left(1+\frac1{x^2}\right)\right)
$$

extends across $O$ and $(0,0)$ to a degree-$2$ [isogeny of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md) with those two points as its kernel. Substitution verifies the target equation, or this follows from the [two-isogeny formula](../../../../../../two-isogeny-formula.md) with $a=0,b=-1$. Both curves are smooth modulo $7$.

For $x=0,1,\ldots,6$, the numbers of affine points with that abscissa on $E$ are $(1,1,0,0,2,2,1)$, and on $E'$ they are $(1,0,2,2,0,0,2)$. Adding the point at infinity gives $8$ on each. The first curve has four rational points of order dividing $2$, from $O$ and the three roots $0,1,-1$. The second has only two: its quadratic factor $X^2+4$ has no root modulo $7$, since $3$ is not a square. By the classification of [finite abelian groups](../../../../../../finite-abelian-group.md),

$$
\boxed{E(\mathbb F_7)\cong\mathbb Z/2\mathbb Z\times\mathbb Z/4\mathbb Z,\qquad E'(\mathbb F_7)\cong\mathbb Z/8\mathbb Z.}
$$

They are thus isogenous with equal orders and nonisomorphic groups.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
