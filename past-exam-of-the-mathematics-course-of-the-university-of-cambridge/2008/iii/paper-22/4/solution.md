<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $g$ be the [Riemannian metric](../../../../../riemannian-metric.md) underlying the [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) and $J$ its compatible [complex structure](../../../../../complex-structure.md). The [fundamental form of a Hermitian manifold](../../../../../fundamental-form-of-a-hermitian-manifold.md) is $\omega(u,v)=g(Ju,v)$. It is a real alternating form of type $(1,1)$. At a point choose an orthonormal real coframe $x^1,y^1,\ldots,x^n,y^n$ adapted to $J$, with $x^j+i y^j$ of type $(1,0)$. Then

$$
\omega=\sum_{j=1}^n x^j\wedge y^j,
\qquad
\boxed{dV_g=x^1\wedge y^1\wedge\cdots\wedge x^n\wedge y^n=\frac{\omega^n}{n!}.}
$$

The orientation here is the complex orientation. In coordinates for which $g=\sum_j((dx^j)^2+(dy^j)^2)$, the same convention reads $\omega=(i/2)\sum_j dz^j\wedge d\bar z^j$.

Use the [complex Hodge star operator](../../../../../complex-hodge-star-operator.md), the complex-linear extension of the real [Hodge star operator](../../../../../hodge-star-operator.md). With the pointwise [Hermitian inner product](../../../../../hermitian-form.md) linear in its first variable, its defining identity is

$$
\alpha\wedge*\bar\beta=\langle\alpha,\beta\rangle_g\,dV_g
$$

for forms of the same total degree. It maps type $(p,q)$ to $(n-q,n-p)$ and satisfies $*^2=(-1)^{p+q}$ in real dimension $2n$. It commutes with [complex conjugation](../../../../../complex-conjugation.md). These conventions distinguish it from the [conjugate-linear Hodge star](../../../../../conjugate-linear-hodge-star.md) $\alpha\mapsto*\bar\alpha$.

Write a top holomorphic-type form as $\eta=a\,\zeta^1\wedge\cdots\wedge\zeta^n$, where $\zeta^j=x^j+i y^j$. On each oriented two-plane, $*x^j=y^j$ and $*y^j=-x^j$, so the two-dimensional star of $\zeta^j$ is $-i\zeta^j$. In taking the star of their product, regrouping complementary one-form factors across the $n$ two-planes contributes $(-1)^{n(n-1)/2}$. Thus the [Hodge star on top holomorphic forms](../../../../../hodge-star-on-top-holomorphic-forms.md) is

$$
*\eta=(-1)^{n(n-1)/2}(-i)^n\eta,
\qquad
\boxed{*\eta=(-1)^{n(n+1)/2}i^n\eta.}
$$

This is pointwise and requires neither holomorphicity of the coefficient $a$ nor closedness of $\omega$.

To compute the [formal adjoint](../../../../../formal-adjoint.md), take compactly supported forms $\alpha$ of degree $k-1$ and $\beta$ of degree $k$. The [Stokes theorem](../../../../../stokes-theorem.md) gives

$$
\int_X d\alpha\wedge*\bar\beta
=(-1)^k\int_X\alpha\wedge d(*\bar\beta).
$$

Since the degree of $d(*\bar\beta)$ is $2n-k+1$, the identity for $*^2$ makes the right side equal to $\int_X\alpha\wedge*\overline{(-*d*\beta)}$. Consequently the [formal adjoint](../../../../../formal-adjoint.md) of $d$ in even real dimension is $d^*=-*d*$. Splitting by type, $-*\partial*$ lowers antiholomorphic degree, while $-*\bar\partial*$ lowers holomorphic degree. Orthogonality of distinct types therefore yields

$$
\boxed{\bar\partial^*=-*\partial*,\qquad
\partial^*=-*\bar\partial*.}
$$

The argument applies locally with compact support, and globally without support restrictions on a compact manifold without boundary.

The [Dolbeault Laplacian](../../../../../dolbeault-laplacian.md) is $\Delta_{\bar\partial}=\bar\partial\bar\partial^*+\bar\partial^*\bar\partial$. A form is $\bar\partial$-harmonic when it lies in its kernel. On a compact [Hermitian manifold](../../../../../hermitian-manifold.md), the adjoint identities imply

$$
\langle\Delta_{\bar\partial}\alpha,\alpha\rangle_{L^2}
=\|\bar\partial\alpha\|_{L^2}^2+\|\bar\partial^*\alpha\|_{L^2}^2.
$$

Thus harmonicity is equivalent to both first-order equations vanishing. The [Dolbeault Hodge decomposition on a compact Hermitian manifold](../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) states that the harmonic space $\mathcal H^{p,q}_{\bar\partial}$ is finite-dimensional and that smooth forms have the orthogonal direct-sum decomposition

$$
\Omega^{p,q}(X)=\mathcal H^{p,q}_{\bar\partial}
\oplus\bar\partial\Omega^{p,q-1}(X)
\oplus\bar\partial^*\Omega^{p,q+1}(X).
$$

To deduce the identification with [Dolbeault cohomology](../../../../../dolbeault-cohomology.md), let $\bar\partial\alpha=0$ and decompose $\alpha=h+\bar\partial u+\bar\partial^*v$. The closedness of $\alpha$ makes it orthogonal to the entire image of $\bar\partial^*$. Taking its inner product with $\bar\partial^*v$ and using the orthogonality of the decomposition gives $\|\bar\partial^*v\|^2=0$. Hence $\alpha=h+\bar\partial u$, so each cohomology class has a harmonic representative. If a harmonic form equals $\bar\partial u$, its squared norm is $\langle\bar\partial^*h,u\rangle=0$, so the representative is unique. We have proved

$$
\boxed{\mathcal H^{p,q}_{\bar\partial}\longrightarrow H^{p,q}_{\bar\partial}(X),\quad h\longmapsto[h],\text{ is an isomorphism}.}
$$

For the complementary types, define $C\alpha=*\bar\alpha$. It maps $(p,q)$ to $(n-p,n-q)$ and is conjugate-linear. If $\alpha$ is harmonic, then $\bar\partial\alpha=0$ and $\partial(*\alpha)=0$ by the adjoint formula. Conjugating the latter equation gives $\bar\partial(*\bar\alpha)=0$. Also, with $k=p+q$,

$$
\bar\partial^*(C\alpha)
=-*\partial*(*\bar\alpha)
=-(-1)^k*\partial\bar\alpha=0,
$$

since $\partial\bar\alpha=\overline{\bar\partial\alpha}$. Therefore $C$ carries harmonic forms to harmonic forms, and $C^2=(-1)^k$ makes it a bijection. This proves [complementary Dolbeault harmonic types on a Hermitian manifold](../../../../../complementary-dolbeault-harmonic-types-on-a-hermitian-manifold.md):

$$
\boxed{\dim_{\mathbb C}\mathcal H^{p,q}_{\bar\partial}
=\dim_{\mathbb C}\mathcal H^{n-p,n-q}_{\bar\partial}.}
$$

The metric supplies a natural conjugate-linear isomorphism. If a complex-linear isomorphism is desired, choose a basis $h_j$ of the first space and send it to the basis $Ch_j$ of the second, extending linearly. This last choice is not canonical; no [Kähler](../../../../../kahler-manifold.md) assumption is needed for either the dimension equality or the harmonic bijection.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
