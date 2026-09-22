<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On $\mathbb C^{n+1}\setminus\{0\}$, let $\Omega=dz_0\wedge\cdots\wedge dz_n$ and let $E=\sum_i z_i\partial_{z_i}$ be the [Euler vector field](../../../../../../euler-vector-field.md). The numerator is its [interior product of a differential form](../../../../../../interior-product.md), so

$$
\alpha=\frac{\iota_E\Omega}{f}.
$$

Both numerator and denominator have homogeneous scaling degree $n+1$. Thus this meromorphic $n$-form is invariant under constant nonzero scalings, and $\iota_E\alpha=0$ makes it horizontal for the quotient to [Complex projective space](../../../../../../complex-projective-space.md).

To check descent using the hint, take a local holomorphic section $Z$ of the quotient and another section $Z'=\lambda Z$, where $\lambda$ is a nowhere-zero [holomorphic function](../../../../../../holomorphic-function.md). In the evaluation

$$
(Z')^*(\iota_E\Omega)(v_1,\ldots,v_n)
=\Omega\bigl(\lambda Z,\lambda\,dZ(v_1)+d\lambda(v_1)Z,\ldots,\lambda\,dZ(v_n)+d\lambda(v_n)Z\bigr),
$$

every term involving $d\lambda$ has two collinear arguments and vanishes. The remaining term is $\lambda^{n+1}Z^*(\iota_E\Omega)$, while $f(\lambda Z)=\lambda^{n+1}f(Z)$. Hence $Z'^*\alpha=Z^*\alpha$. The forms therefore glue to a meromorphic section of the [canonical bundle](../../../../../../canonical-bundle.md) of [Complex projective space](../../../../../../complex-projective-space.md).

On the affine chart $z_j\ne0$, use the section $z_j=1$ and list the remaining coordinates as $t_1,\ldots,t_n$ in increasing original-index order. If $F$ is the resulting polynomial, then

$$
\alpha=(-1)^j\frac{dt_1\wedge\cdots\wedge dt_n}{F}.
$$

At a point of $Y$, some derivative $F_{t_r}$ is nonzero. Otherwise all the homogeneous derivatives except possibly $f_{z_j}$ would vanish; the [Euler homogeneous function theorem](../../../../../../euler-theorem-for-homogeneous-functions.md) gives $\sum_i z_if_{z_i}=(n+1)f=0$ there, forcing $f_{z_j}=0$ too. This contradicts the permitted smoothness criterion. The [holomorphic inverse function theorem](../../../../../../holomorphic-inverse-function-theorem.md) now makes $F$ a transverse coordinate, so the pole is simple. On a neighbourhood with $F_{t_r}\ne0$, rearranging the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md) gives

$$
\alpha=\frac{dF}{F}\wedge
\frac{(-1)^{j+r-1}}{F_{t_r}}\,dt_1\wedge\cdots\wedge\widehat{dt_r}\wedge\cdots\wedge dt_n.
$$

By part (a), its [Poincaré residue](../../../../../../poincare-residue-along-a-smooth-hypersurface.md) is consequently

$$
\boxed{\operatorname{Res}_Y(\alpha)=
\left.\frac{(-1)^{j+r-1}}{F_{t_r}}\,dt_1\wedge\cdots\wedge\widehat{dt_r}\wedge\cdots\wedge dt_n\right|_Y.}
$$

The remaining $t$ coordinates form a [holomorphic coordinate](../../../../../../holomorphic-coordinate.md) system on $Y$, and $F_{t_r}$ is nonzero in this neighbourhood. The displayed top form is therefore nowhere zero. These neighbourhoods cover $Y$ and part (a) guarantees agreement on their overlaps. **The residue is a nowhere-vanishing global holomorphic section**:

$$
\boxed{K_Y\cong\mathcal O_Y.}
$$

This is the explicit [residue trivialization for a degree n+1 projective hypersurface](../../../../../../residue-trivialization-for-a-degree-n-plus-1-projective-hypersurface.md), consistent with the [adjunction formula](../../../../../../adjunction-formula.md) $K_Y\cong\mathcal O_Y((n+1)-n-1)$, but obtained here directly from the indicated form.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
