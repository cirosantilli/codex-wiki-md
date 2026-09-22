<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use real [differential forms](../../../../../differential-form-split.md) and the usual convention that a [smooth manifold](../../../../../smooth-manifold.md) has no boundary unless one is specified. On a noncompact manifold the formal-adjoint identity below uses compactly supported forms. On a compact manifold it has no boundary contribution; if a boundary were allowed, extra boundary conditions would be necessary.

The [Riemannian metric](../../../../../riemannian-metric.md) gives the dual [inner product](../../../../../inner-product.md) on $T_x^*M$ and hence the [inner product on exterior powers of a cotangent space](../../../../../inner-product-on-exterior-powers-of-a-cotangent-space.md):

$$
\boxed{\langle\xi_1\wedge\cdots\wedge\xi_p,\zeta_1\wedge\cdots\wedge\zeta_p\rangle=\det\bigl(\langle\xi_i,\zeta_j\rangle\bigr).}
$$

Extend this bilinearly. Equivalently, the increasing wedge products of an orthonormal coframe are an orthonormal basis of $\Lambda^pT_x^*M$. The [Hodge star operator](../../../../../hodge-star-operator.md) is the unique map $*:\Lambda^pT_x^*M\to\Lambda^{n-p}T_x^*M$ satisfying $\alpha\wedge*\beta=\langle\alpha,\beta\rangle\operatorname{vol}_g$. If $e^1,\ldots,e^n$ is a positively oriented orthonormal coframe, $*e^I=\varepsilon(I,I^c)e^{I^c}$. Moving the $p$ factors of $I$ across the $n-p$ factors of its complement changes the sign by $(-1)^{p(n-p)}$, so

$$
\boxed{*^2\alpha=(-1)^{p(n-p)}\alpha.}
$$

The basis formula also proves that $*$ is an isometry.

For $\beta\in\Omega^{p-1}(M)$ and $\alpha\in\Omega^p(M)$ with compactly supported product, the [Stokes theorem](../../../../../stokes-theorem.md) and the [Leibniz rule](../../../../../leibniz-rule.md) for the [exterior derivative](../../../../../exterior-derivative.md) give

$$
0=\int_Md(\beta\wedge*\alpha)=\int_Md\beta\wedge*\alpha+(-1)^{p-1}\int_M\beta\wedge d*\alpha.
$$

Thus $(d\beta,\alpha)_{L^2}=(-1)^p\int_M\beta\wedge d*\alpha$. The formal [adjoint operator](../../../../../adjoint-operator.md) $\delta$ satisfies $*\delta\alpha=(-1)^p d*\alpha$. Applying the inverse star and its square on degree $p-1$ gives the [codifferential](../../../../../codifferential.md)

$$
\boxed{\delta|_{\Omega^p}=(-1)^{n(p+1)+1}*d*.}
$$

The exponent is congruent to $p+(p-1)(n-p+1)$ modulo two, so this convention is consistent in every degree. Define the [Hodge Laplacian](../../../../../hodge-laplacian.md) by $\Delta=d\delta+\delta d$ and a [harmonic differential form](../../../../../harmonic-differential-form.md) by $\Delta\alpha=0$. On a compact manifold,

$$
(\Delta\alpha,\alpha)_{L^2}=\|d\alpha\|_{L^2}^2+\|\delta\alpha\|_{L^2}^2.
$$

Both nonnegative terms vanish for a harmonic form, giving **$d\alpha=\delta\alpha=0$**. Conversely these two equations imply harmonicity.

Now let $n=4$. The printed eigenvalue relation omits the subscript on its right-hand side; the intended equation is $*\alpha_\pm=\pm\alpha_\pm$. On two-forms $*^2=1$, so

$$
\boxed{\alpha_+=\tfrac12(\alpha+*\alpha),\qquad\alpha_-=\tfrac12(\alpha-*\alpha).}
$$

These are respectively [self-dual two-forms](../../../../../self-dual-differential-form.md) and [anti-self-dual two-forms](../../../../../anti-self-dual-differential-form.md), and sum to $\alpha$. Their uniqueness follows because the $+1$ and $-1$ eigenspaces have zero intersection. Star is an orthogonal involution here, hence is self-adjoint and its opposite eigenspaces are orthogonal.

For closed two-forms define $Q([\alpha],[\beta])=\int_N\alpha\wedge\beta$. Adding $d\xi$ to $\alpha$ changes the integral by $\int_Nd(\xi\wedge\beta)=0$; adding an exact form to $\beta$ has the same effect. This is the [real de Rham intersection form in dimension four](../../../../../real-de-rham-intersection-form-in-dimension-four.md). The [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md) in degrees two and two is symmetric because $(-1)^{2\cdot2}=1$; hence $Q$ is a symmetric bilinear form on $H_{\mathrm{dR}}^2(N;\mathbb R)$.

In four dimensions $\delta=-*d*$ in every degree. If $h$ is a harmonic two-form, $\delta h=0$ gives $d*h=0$, and $dh=0$ gives $\delta*h=-*dh=0$. Thus $*h$ is harmonic, and $\mathcal H^2=\mathcal H^+\oplus\mathcal H^-$ is the harmonic star-eigenspace decomposition. Use the permitted unique harmonic representative for each [de Rham cohomology](../../../../../de-rham-cohomology.md) class. For harmonic $h,k$,

$$
Q(h,k)=(h,*k)_{L^2}= (h_+,k_+)_{L^2}-(h_-,k_-)_{L^2}.
$$

The mixed terms vanish by orthogonality. The first restriction is positive definite and the second negative definite. In particular a nonzero harmonic $h$ has $Q(h,*h)=\|h\|_{L^2}^2>0$, proving nondegeneracy. Hence the [signature of the intersection form from harmonic duality](../../../../../signature-of-the-intersection-form-from-harmonic-duality.md) is

$$
\boxed{\operatorname{signature}Q=(b^+(N),b^-(N)),\qquad b^\pm(N)=\dim\mathcal H^\pm(N).}
$$

The finite dimensions and the harmonic description also follow from the [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md).

For completeness, the [Hodge decomposition theorem](../../../../../hodge-decomposition-theorem.md) on a compact oriented [Riemannian manifold](../../../../../riemannian-manifold.md) without boundary states the finite-dimensional harmonic space and the $L^2$-orthogonal direct sum

$$
\boxed{\Omega^p=\mathcal H^p\oplus d\Omega^{p-1}\oplus\delta\Omega^{p+1}.}
$$

The three summand components are unique, although their potentials need not be. Given an exact three-form $\beta=d\omega$ on $N$, decompose its smooth two-form potential as $\omega=h+d\xi+\delta\psi$, with $\psi\in\Omega^3$. Since $dh=0$ and $d^2=0$, $\beta=d\delta\psi$. Put $a=\delta\psi$. In dimension four, $a=-*d*\psi$, and $*^2=1$ on two-forms gives $*a=-d*\psi$, so $d*a=0$. Consequently

$$
\boxed{\sigma=a+*a=\delta\psi+*\delta\psi,\qquad *\sigma=\sigma,\qquad d\sigma=\beta.}
$$

This constructs a [self-dual primitive of an exact three-form](../../../../../self-dual-primitive-of-an-exact-three-form.md). The sum contains no factor $1/2$: it is twice the self-dual projection of the coexact potential. Using the unscaled projection alone would give $d\sigma=\beta/2$. This proves the final unheaded request.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
