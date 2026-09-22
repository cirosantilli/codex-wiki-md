<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Represent a transformation by

$$
M(u,v)=\begin{pmatrix}u&v\\\overline v&\overline u\end{pmatrix},\qquad\det M=|u|^2-|v|^2=1.
$$

Multiplication preserves this form and [determinant](../../../../../determinant.md), and the inverse has the same form with parameters $(\overline u,-v)$. To check the congruence condition, [complex conjugation](../../../../../complex-conjugation.md) is the identity modulo $2\mathbb Z[i]$. Thus $u+v\equiv1$ says exactly that $M$ fixes the column $(1,1)^T$ modulo two. Products and inverses preserve this property. The identity belongs to the set, and changing the common sign of $(u,v)$ does not change either the transformation or its congruence. Hence **these transformations form a [group](../../../../../group-split.md)**.

Because $|u|>|v|$, the denominator has no zero in the disc. Direct calculation gives

$$
1-|g(z)|^2=\frac{1-|z|^2}{|\overline vz+\overline u|^2},\qquad
|g'(z)|=\frac1{|\overline vz+\overline u|^2}.
$$

The inverse also maps the disc into itself, so $g$ is a disc automorphism, and these identities show that it preserves the [hyperbolic metric](../../../../../hyperbolic-metric.md) $2|dz|/(1-|z|^2)$.

The action is properly discontinuous. If $C\subset\mathbb D$ is [compact](../../../../../compact-space.md), put $R=\max_{z\in C}\rho(0,z)$. If $gC\cap C\ne\varnothing$, choose $z,w\in C$ with $w=gz$. Then

$$
\rho(0,g0)\le\rho(0,w)+\rho(w,g0)=\rho(0,w)+\rho(z,0)\le2R.
$$

Since $g0=v/\overline u$ and $|u|^2-|v|^2=1$, its distance bound gives $|v/u|\le\tanh R<1$ and therefore $|u|^2=1/(1-|v/u|^2)\le\cosh^2R$. There are only finitely many [Gaussian integers](../../../../../gaussian-integer.md) $u,v$ with these bounds, so only finitely many $g$ satisfy $gC\cap C\ne\varnothing$. This proves the required [properly discontinuous group action](../../../../../properly-discontinuous-group-action.md) directly.

If $g0=0$, then $v=0$ and $u$ is one of the [Gaussian units](../../../../../gaussian-units.md) $1,-1,i,-i$. The congruence $u-1\in2\mathbb Z[i]$ leaves only $u=\pm1$. Both give the identity transformation. Thus **the [point stabilizer](../../../../../stabilizer-subgroup.md) of zero is trivial**.

The closed [Dirichlet region](../../../../../dirichlet-domain.md) centered at zero is the set of $z$ with $\rho(z,0)\le\rho(z,g0)$ for every $g$. For a nonidentity element, $v\ne0$. Write

$$
N=|v|^2\in\mathbb Z_{\ge1},\qquad uv=m+in,\qquad
q=g0=\frac{uv}{|u|^2}=\frac{m+in}{N+1}.
$$

The distance inequality is equivalent, by [pseudohyperbolic distance](../../../../../pseudohyperbolic-distance.md), to $|z|\le|(z-q)/(1-\overline qz)|$. Squaring and subtracting yields

$$
|z-q|^2-|z|^2|1-\overline qz|^2
=(1-|z|^2)\bigl[|q|^2(1+|z|^2)-2\operatorname{Re}(z\overline q)\bigr].
$$

Since $|z|<1$ and $|q|^2=N/(N+1)$, the bisector half-plane is exactly

$$
2(mx+ny)\le N(1+x^2+y^2),\qquad z=x+iy.
$$

For $u=1+i$ or $1-i$ and $v=i$ or $-i$, all the [group](../../../../../group-split.md) conditions hold and the products $uv$ are the four numbers $\pm1\pm i$, with $N=1$. Their four inequalities force

$$
2(|x|+|y|)\le1+x^2+y^2.
$$

Conversely, for any [group](../../../../../group-split.md) element $m^2+n^2=|uv|^2=N(N+1)<(N+1)^2$. As $m,n$ are integers, $|m|,|n|\le N$. Thus every point satisfying those four inequalities satisfies every other one:

$$
2(mx+ny)\le2N(|x|+|y|)\le N(1+x^2+y^2).
$$

This proves, with no missing bisectors, the [Gaussian-integer disc group with an ideal-square Dirichlet domain](../../../../../gaussian-integer-disc-group-with-an-ideal-square-dirichlet-domain.md) formula

$$
\boxed{D_G(0)=\{x+iy:x^2+y^2<1,\ 2(|x|+|y|)\le1+x^2+y^2\}.}
$$

Equivalently it is the part of the [unit disc](../../../../../unit-disc.md) outside all four open circles of radius one centered at $1+i,1-i,-1+i,-1-i$. Its sides are the inward arcs of those circles. They meet the unit circle orthogonally, and their ideal vertices are $\boxed{1,i,-1,-i}$; these vertices themselves lie outside the open disc.

<a id="5/image-origin-centered-dirichlet-region-and-the-four-neighboring-orbit-points"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-11-dirichlet-region.png)

**[Figure 1](#5/image-origin-centered-dirichlet-region-and-the-four-neighboring-orbit-points). Origin-centered Dirichlet region and the four neighboring orbit points**.

The origin has trivial [point stabilizer](../../../../../stabilizer-subgroup.md) and the [group orbit](../../../../../orbit-of-a-group-action.md) is locally finite by the discontinuity proof, so this closed bisector intersection has translates covering the disc with disjoint interiors, as in the definition of a [Dirichlet domain](../../../../../dirichlet-domain.md). Side identifications are allowed on its boundary.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
