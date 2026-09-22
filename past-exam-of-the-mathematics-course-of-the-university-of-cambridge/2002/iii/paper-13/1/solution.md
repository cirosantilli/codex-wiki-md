<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $X$ be a connected [compact Riemann surface](../../../../../compact-riemann-surface.md) of [genus](../../../../../genus-of-a-surface.md) $g$. Choose an oriented [symplectic basis](../../../../../symplectic-basis.md) $a_1,\ldots,a_g,b_1,\ldots,b_g$ of $H_1(X,\mathbb Z)$, with $a_i\cdot b_j=\delta_{ij}$. For a closed complex [differential form](../../../../../differential-form-split.md) $\alpha$, write $A_i(\alpha)=\int_{a_i}\alpha$ and $B_i(\alpha)=\int_{b_i}\alpha$. The [Riemann bilinear relations](../../../../../riemann-bilinear-relations-for-a-compact-surface.md) begin with the identity

$$
\int_X\alpha\wedge\beta=\sum_{i=1}^g\bigl(A_i(\alpha)B_i(\beta)-B_i(\alpha)A_i(\beta)\bigr).
$$

To prove it, cut $X$ along the chosen cycles to obtain a fundamental polygon $P$. On this simply connected polygon, a closed [differential form](../../../../../differential-form-split.md) has a primitive $F$, with $dF=\alpha$. [Stokes theorem](../../../../../stokes-theorem.md) gives $\int_P\alpha\wedge\beta=\int_{\partial P}F\beta$. The two copies of each edge have opposite orientations, and their values of $F$ differ by the period acquired in passing between them. Pairing the copies of the $a_i$ and $b_i$ edges gives, respectively, $-B_i(\alpha)A_i(\beta)$ and $A_i(\alpha)B_i(\beta)$. Summing proves the identity; the convention $a_i\cdot b_i=1$ fixes its sign.

For [holomorphic one-forms](../../../../../holomorphic-one-form.md) $\omega,\eta$, their [wedge product](../../../../../exterior-product.md) is zero because locally both are multiples of $dz$. Thus the first [holomorphic](../../../../../complex-differentiability-at-a-point.md) [Riemann bilinear relations](../../../../../riemann-bilinear-relations-for-a-compact-surface.md) is

$$
\sum_i\bigl(A_i(\omega)B_i(\eta)-B_i(\omega)A_i(\eta)\bigr)=0.
$$

For a nonzero [holomorphic one-form](../../../../../holomorphic-one-form.md) $\omega=f(z)\,dz$, the second relation follows by applying the bilinear identity to $\omega,\overline\omega$:

$$
i\sum_i\bigl(A_i(\omega)\overline{B_i(\omega)}-B_i(\omega)\overline{A_i(\omega)}\bigr)
=i\int_X\omega\wedge\overline\omega
=2\int_X|f|^2\,dx\,dy>0.
$$

In particular, a [holomorphic one-form](../../../../../holomorphic-one-form.md) with all $a$-periods zero must vanish. Since $\dim H^0(X,K_X)=g$, the map taking a [holomorphic one-form](../../../../../holomorphic-one-form.md) to its $a$-periods is an [isomorphism](../../../../../isomorphism.md). We can therefore choose normalized [holomorphic one-forms](../../../../../holomorphic-one-form.md) $\omega_1,\ldots,\omega_g$ with $\int_{a_i}\omega_j=\delta_{ij}$. Put $B_{ij}=\int_{b_i}\omega_j$. The first relation applied to $\omega_j,\omega_k$ gives $B_{jk}=B_{kj}$, and the second applied to $\sum_jc_j\omega_j$ gives $2\overline c^{,t}(\operatorname{Im}B)c>0$ for $c\ne0$. Consequently

$$
\boxed{B=B^t,\qquad Y=\operatorname{Im}B>0.}
$$

These conclusions make the construction of the [Jacobian variety](../../../../../jacobian-variety.md) work. Integration identifies the image of $H_1(X,\mathbb Z)$ in $H^0(X,K_X)^*$ with the [period lattice](../../../../../period-lattice.md) $\Lambda=\mathbb Z^g+B\mathbb Z^g$. The real-linear map $(m,n)\mapsto m+Bn$ is invertible: its imaginary part is $Yn$, and $Y$ is invertible. Hence $\Lambda$ is a discrete lattice of full real [rank](../../../../../rank-one-quadratic-form.md) $2g$, and

$$
\boxed{\operatorname{Jac}(X)=H^0(X,K_X)^*/H_1(X,\mathbb Z)\simeq\mathbb C^g/(\mathbb Z^g+B\mathbb Z^g)}
$$

is a [compact](../../../../../compact-space.md) [complex torus](../../../../../complex-torus.md), rather than a non-Hausdorff quotient. Changing the [symplectic basis](../../../../../symplectic-basis.md) changes the displayed coordinates but not this intrinsic quotient.

The [Riemann bilinear relations](../../../../../riemann-bilinear-relations-for-a-compact-surface.md) also supply its [polarization of a complex torus](../../../../../polarization-of-a-complex-torus.md). Use the [Hermitian form](../../../../../hermitian-form.md) $H(z,w)=z^tY^{-1}\overline w$, linear in the first argument, and set $E=-\operatorname{Im}H$. Symmetry of $B$ gives

$$
E(m+Bn,m'+Bn')=m^tn'-n^tm',\qquad E(v,iv)=H(v,v)>0.
$$

Thus $E$ is an integral positive [Riemann form on a complex torus](../../../../../riemann-form-on-a-complex-torus.md). Its matrix on the displayed lattice basis is the unimodular [symplectic matrix](../../../../../symplectic-matrix.md). The corresponding positive [holomorphic line bundle](../../../../../holomorphic-line-bundle.md), equivalently the one constructed from theta automorphy in Solution 4, gives a principal [polarization of a complex torus](../../../../../polarization-of-a-complex-torus.md). By the [Kodaira embedding theorem](../../../../../kodaira-embedding-theorem.md) this makes the [complex torus](../../../../../complex-torus.md) projective, hence an [abelian variety](../../../../../abelian-variety-split.md). The normalization $E=-\operatorname{Im}H$ here is important because $H$ was chosen linear in its first argument. If $g=0$, the spaces of [holomorphic one-forms](../../../../../holomorphic-one-form.md) and periods are zero and the [Jacobian variety](../../../../../jacobian-variety.md) is a point.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
