<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [exterior derivative](../../../../../exterior-derivative.md) is the real-linear degree-one operator $d:\Omega^k\to\Omega^{k+1}$ characterized by its usual derivative on functions, the [graded Leibniz rule](../../../../../graded-leibniz-rule.md)

$$
d(\alpha\wedge\beta)=d\alpha\wedge\beta+(-1)^k\alpha\wedge d\beta\quad(\alpha\in\Omega^k),
$$

and $d^2=0$. In local coordinates,

$$
d\left(\sum_I f_I\,dx^{i_1}\wedge\cdots\wedge dx^{i_k}\right)
=\sum_I df_I\wedge dx^{i_1}\wedge\cdots\wedge dx^{i_k}.
$$

These rules determine it uniquely, and the coordinate formula shows its existence and invariance under coordinate changes. It also commutes with [pullback of a differential form](../../../../../pullback-of-a-differential-form.md).

On the unit ball let $V=x^i\partial_i$ be the radial [vector field](../../../../../vector-field.md), and let $F_t(x)=tx$. For $k\ge1$ define the [radial homotopy operator](../../../../../radial-homotopy-operator.md) by

$$
(h_k\omega)_x(v_1,\ldots,v_{k-1})
=\int_0^1 t^{k-1}\omega_{tx}(x,v_1,\ldots,v_{k-1})\,dt.
$$

Here the vectors are identified using the ambient Euclidean coordinates. Equivalently $h_k\omega=\int_0^1t^{-1}F_t^*(\iota_V\omega)\,dt$, where $\iota_V$ is the [interior product](../../../../../interior-product.md). The apparent factor $t^{-1}$ is harmless: the coordinate coefficients of its integrand contain $t^{k-1}$, so the integral is smooth at $t=0$ and depends smoothly on $x$. This is a linear map to $\Omega^{k-1}$; set $h_0=0$.

For $t>0$, differentiation of the coordinate pullback and [Cartan's magic formula](../../../../../cartan-s-magic-formula.md) give

$$
\frac{d}{dt}F_t^*\omega
=t^{-1}F_t^*\mathcal L_V\omega
=t^{-1}F_t^*(d\iota_V\omega+\iota_Vd\omega).
$$

For completeness, Cartan’s identity follows by checking it on functions and coordinate one-forms: both sides give $V(f)$ on $f$ and $d(V(x^i))$ on $dx^i$. Both are degree-zero derivations of the exterior algebra, so the checks imply the identity on every local form. Integrating from zero to one proves

$$
\boxed{dh_k\omega+h_{k+1}d\omega=\omega-F_0^*\omega.}
$$

For positive $k$, the pullback by the constant map is zero, so this is the required identity. If $d\omega=0$ and $k\ge1$, it follows that $\omega=d(h_k\omega)$. A chart about any point contains such a ball, proving the [Poincaré lemma](../../../../../poincare-lemma.md). In degree zero the formula is instead $h_1df=f-f(0)$: a constant function cannot be the image of the uncorrected homotopy identity. This [degree-zero correction to radial homotopy](../../../../../degree-zero-correction-to-radial-homotopy.md) specifies the necessary positive-degree convention in the printed request.

To treat the sphere, cover $S^2$ by the complements of its north and south poles. Each is diffeomorphic to $\mathbb R^2$, where the same star-shaped homotopy applies. A [closed differential one-form](../../../../../closed-differential-one-form.md) $\alpha$ therefore has local primitives $f_N$ and $f_S$. On their overlap $d(f_N-f_S)=0$. This overlap is connected, so the difference is a constant $c$. Replacing $f_N$ by $f_N-c$ makes the primitives agree, and they glue smoothly to a global function. Thus

$$
\boxed{\alpha=df\text{ on }S^2,\qquad H^1_{\mathrm{dR}}(S^2)=0.}
$$

This proves directly that [closed one-forms on the two-sphere are exact](../../../../../closed-one-forms-on-the-two-sphere-are-exact.md).

For the [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md), assume a compact oriented [Riemannian manifold](../../../../../riemannian-manifold.md) without boundary. The [Hodge star operator](../../../../../hodge-star-operator.md) is characterized by $\alpha\wedge*\beta=\langle\alpha,\beta\rangle\operatorname{vol}_g$ and obeys $**\alpha=(-1)^{k(n-k)}\alpha$. The formal $L^2$ adjoint of $d$ on $k$-forms is $\delta=(-1)^{n(k+1)+1}*d*$. Define the [Hodge Laplacian](../../../../../hodge-laplacian.md) $\Delta=d\delta+\delta d$ and the space $\mathcal H^k=\ker\Delta$ of [harmonic differential forms](../../../../../harmonic-differential-form.md). Integration by parts, with no boundary term, gives

$$
\langle\Delta\alpha,\alpha\rangle_{L^2}
=\|d\alpha\|_{L^2}^2+\|\delta\alpha\|_{L^2}^2.
$$

Hence a form is harmonic exactly when it is both closed and coclosed. The [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md) states that $\mathcal H^k$ is finite-dimensional and that there is the orthogonal decomposition

$$
\Omega^k(M)=\mathcal H^k\oplus d\Omega^{k-1}(M)\oplus\delta\Omega^{k+1}(M).
$$

If a closed form has decomposition $\alpha=h+d\beta+\delta\gamma$, then $\langle\alpha,\delta\gamma\rangle=\langle d\alpha,\gamma\rangle=0$. Orthogonality consequently forces $\delta\gamma=0$, so its [de Rham cohomology](../../../../../de-rham-cohomology.md) class is represented by $h$. An exact harmonic form $h=d\beta$ has $\|h\|^2=\langle\delta h,\beta\rangle=0$, proving uniqueness. Thus

$$
\boxed{\mathcal H^k(M)\cong H^k_{\mathrm{dR}}(M).}
$$

Every top-degree form is $\omega=f\operatorname{vol}_g$, and $d\omega=0$ for dimensional reasons. Its [Hodge star](../../../../../hodge-star-operator.md) is $f$, so the formula for $\delta$ shows that $\delta\omega=0$ exactly when $df=0$. On a connected manifold this says that $f$ is constant. Therefore the [harmonic top-degree forms on a closed oriented manifold](../../../../../harmonic-top-degree-forms-on-a-closed-oriented-manifold.md) form the space

$$
\boxed{\mathcal H^n(M)=\mathbb R\,\operatorname{vol}_g,\qquad\dim\mathcal H^n(M)=1.}
$$

Any such smooth manifold admits a [Riemannian metric](../../../../../riemannian-metric.md); the assertion is valid for every choice of that metric.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
