<h1 id="25g/solution">Solution</h1>

↑ **Parent:** [25G](../25g.md)

Let $X\subseteq\mathbb A^n$ have ideal $I(X)$, and let $p\in X$. Its [Zariski tangent space](../../../../../zariski-tangent-space.md) is

$$
T_pX
=\left\{v\in k^n:
\sum_{j=1}^n\frac{\partial f}{\partial x_j}(p)v_j=0
\text{ for every }f\in I(X)\right\}.
$$

If $X$ is irreducible, $p$ is smooth when

$$
\dim T_pX=\dim X;
$$

otherwise it is singular. Equivalently, for generators of $I(X)$, the [Jacobian](../../../../../jacobian-matrix.md) has the maximum rank $n-\dim X$ at $p$.

Now let the irreducible affine plane cubic be $X=V(f)\subseteq\mathbb A^2$. Suppose distinct points $p,q\in X$ were both singular. Parametrize their joining line by

$$
\ell(t)=p+t(q-p)
$$

and put $h(t)=f(\ell(t))$. Then $\deg h\leq3$. At $t=0$,

$$
h(0)=0,
\qquad
h'(0)=\nabla f(p)\mathbin\cdot(q-p)=0,
$$

so zero is a root of multiplicity at least two. The same argument at $t=1$ gives another root of multiplicity at least two. Therefore $h$ has at least four roots counted with multiplicity and must vanish identically. The line through $p,q$ is then contained in $X$, so its linear equation divides $f$, contradicting irreducibility. This proves [singular points of an irreducible affine plane cubic](../../../../../singular-points-of-an-irreducible-affine-plane-cubic.md) are unique when they exist.

For the density statement, embed an irreducible affine variety $X$ of dimension $d$ in $\mathbb A^n$ and choose generators $f_1,\ldots,f_r$ of its ideal. By [dimension from minimum tangent dimension](../../../../../dimension-from-minimum-tangent-dimension.md), some point has tangent dimension $d$, so the Jacobian has rank $n-d$ there. Some $(n-d)\times(n-d)$ minor $\Delta$ is consequently nonzero on $X$. The distinguished open set

$$
X_\Delta=\{p\in X:\Delta(p)\ne0\}
$$

is nonempty, and at each of its points the Jacobian rank is at least $n-d$. Since every tangent space has dimension at least $d$, the rank is also at most $n-d$. Thus every point of $X_\Delta$ is smooth. A nonempty open subset of an [irreducible topological space](../../../../../irreducible-topological-space.md) is dense, proving [density of the smooth locus](../../../../../density-of-the-smooth-locus.md).

Finally write the smooth irreducible [projective hypersurface](../../../../../projective-hypersurface.md) as

$$
X=V_+(F)\subseteq\mathbb P^n
$$

for an irreducible homogeneous polynomial $F$. The closure of $\pi^{-1}(X)$ is its [affine cone over a projective hypersurface](../../../../../affine-cone-over-a-projective-hypersurface.md)

$$
Y=V(F)\subseteq\mathbb A^{n+1}.
$$

At a nonzero point $y\in Y$, simultaneous vanishing of all partial derivatives of $F$ would make the projective point $[y]\in X$ singular. Since $X$ is smooth, this cannot happen. Hence every nonzero point of $Y$ is smooth, and the origin is its only possible singular point.

Both possibilities occur. If $X$ is a projective hyperplane, then $F$ is linear and $Y$ is an affine linear subspace, hence smooth even at the origin. For a singular cone, take the smooth conic

$$
X=V_+(x_0x_2-x_1^2)\subseteq\mathbb P^2.
$$

Its affine cone is

$$
Y=V(x_0x_2-x_1^2)\subseteq\mathbb A^3.
$$

All first derivatives vanish at the origin, so the vertex is singular, while the preceding argument shows that it is the only singular point.

## ↑ Ancestors (10)

1. [25G](../25g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
