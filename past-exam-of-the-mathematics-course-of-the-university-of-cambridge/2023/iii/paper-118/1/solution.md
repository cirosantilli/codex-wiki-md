<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $(z^1,\ldots,z^n)$ be a [complex manifold](../../../../../complex-manifold.md) chart, with $z^j=x^j+iy^j$. The [almost complex structure induced by a complex atlas](../../../../../almost-complex-structure-induced-by-a-complex-atlas.md) is

$$
J\frac{\partial}{\partial x^j}=\frac{\partial}{\partial y^j},
\qquad
J\frac{\partial}{\partial y^j}=-\frac{\partial}{\partial x^j}.
$$

Thus $J^2=-I$. On an overlap, the derivative of a [holomorphic map](../../../../../holomorphic-map.md) is complex linear and hence commutes with multiplication by $i$. The two coordinate definitions of $J$ therefore agree, so $J$ is globally well-defined.

The complexified cotangent bundle splits into the $i$- and $-i$-eigenspaces of $J^*$, locally spanned by $dz^j$ and $d\bar z^j$. A [differential form of type (p, q)](../../../../../differential-form-of-type-p-q.md) is a sum

$$
\alpha=\sum_{|I|=p,\,|K|=q}\alpha_{I\bar K}\,dz^I\wedge d\bar z^K.
$$

Splitting the [exterior derivative](../../../../../exterior-derivative.md) according to type defines

$$
d=\partial+\bar\partial,
\qquad
\partial:\Omega^{p,q}\to\Omega^{p+1,q},
\qquad
\bar\partial:\Omega^{p,q}\to\Omega^{p,q+1}.
$$

Complex conjugation sends $dz^j$ to $d\bar z^j$ and conjugates the coefficient derivatives. Term by term this gives the [complex conjugation of differential-form type](../../../../../complex-conjugation-of-differential-form-type.md) identity

$$
\bar\partial\bar\alpha=\overline{\partial\alpha}.
$$

Let $J$ act on a $k$-form by

$$
(J\alpha)(v_1,\ldots,v_k)=\alpha(Jv_1,\ldots,Jv_k).
$$

It acts on a $(p,q)$-form by $i^{p-q}$. Therefore $J^{-1}dJ$ multiplies the $\partial$ component by $-i$ and the $\bar\partial$ component by $i$, proving the [d c operator](../../../../../d-c-operator.md) formula

$$
J^{-1}dJ=i(\bar\partial-\partial)=d^c.
$$

A [holomorphic vector field](../../../../../holomorphic-vector-field.md) is a holomorphic section of $T^{1,0}X$. On the affine chart $U_0\subset\mathbb{CP}^n$, put $w_k=z_k/z_0$. The projection is

$$
\varphi_0(z)=(1,w_1,\ldots,w_n).
$$

Direct differentiation gives

$$
(d\varphi_0)_a\left(\frac{\partial}{\partial z_j}\right)
=
\begin{cases}
\displaystyle \frac1{a_0}\frac{\partial}{\partial w_j},&j\ne0,\\[6pt]
\displaystyle-\frac1{a_0^2}\sum_{k=1}^na_k\frac{\partial}{\partial w_k},&j=0.
\end{cases}
$$

If $\xi(z)$ is linear and homogeneous, the pushed-forward coefficients are consequently $\xi(1,w)$ when $j\ne0$, and $-\xi(1,w)w_k$ when $j=0$. They are holomorphic on $U_0$.

More intrinsically, $\xi(z)\partial_{z_j}$ is a linear vector field $Az$ on $\mathbb C^{n+1}$. Its flow $e^{tA}$ preserves complex lines and induces the projective transformations

$$
[z]\longmapsto[e^{tA}z].
$$

Differentiating gives a globally defined [projectivization of a linear vector field](../../../../../projectivization-of-a-linear-vector-field.md), whose expression on $U_0$ is the field just computed. This proves extension across the other affine charts.

Finally choose distinct complex numbers $\lambda_0,\ldots,\lambda_n$ and the diagonal field

$$
Z=\sum_{j=0}^n\lambda_jz_j\frac{\partial}{\partial z_j}.
$$

Its projectivization vanishes at $[z]$ precisely when $(\lambda_0z_0,\ldots,\lambda_nz_n)$ is proportional to $z$, so $[z]$ is an eigenline. The distinct eigenvalues leave exactly the $n+1$ coordinate points. Hence $\mathbb{CP}^n$ has a holomorphic vector field with finitely many zeroes.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
