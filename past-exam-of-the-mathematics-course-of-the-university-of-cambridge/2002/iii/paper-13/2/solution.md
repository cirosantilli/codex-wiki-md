<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Fix $p_0\in X$ and use the normalized [holomorphic one-forms](../../../../../holomorphic-one-form.md) and [period lattice](../../../../../period-lattice.md) of Solution 1. The [Abel-Jacobi map of a compact Riemann surface](../../../../../abel-jacobi-map-of-a-compact-riemann-surface.md) is

$$
u(p)=\left(\int_{p_0}^p\omega_1,\ldots,\int_{p_0}^p\omega_g\right)\pmod\Lambda.
$$

Changing paths changes the vector by a period, so this is well defined and [holomorphic](../../../../../complex-differentiability-at-a-point.md). Adding these vectors gives a symmetric map on $X^d$ and therefore the [Abelian sum map](../../../../../abel-map-of-an-algebraic-curve.md) $u_d:X^{(d)}\to\operatorname{Jac}(X)$. Locally, even where points coincide, symmetric [holomorphic functions](../../../../../holomorphic-function.md) descend to the elementary symmetric coordinates of the [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md). For any [divisor](../../../../../divisor.md) $D=\sum_pn_pp$ of degree zero, define $u(D)=\sum_pn_pu(p)$. **[Abel's theorem](../../../../../abel-theorem-for-divisors.md) says that $D$ is a [principal divisor](../../../../../principal-divisor-on-an-algebraic-curve.md) if and only if $u(D)=0$.** Equivalently, two effective [divisors](../../../../../divisor.md) of the same degree have the same Abel sum exactly when they are [linearly equivalent](../../../../../linear-equivalence-of-weil-divisors.md).

We first establish the [residue](../../../../../residue.md) version of the bilinear identity. Let $\eta$ be a [meromorphic differential on a Riemann surface](../../../../../meromorphic-differential-on-a-riemann-surface.md) with only simple poles and total [residue](../../../../../residue.md) zero, and let $F=\int_{p_0}^p\omega$ on the cut polygon, for a [holomorphic one-form](../../../../../holomorphic-one-form.md) $\omega$. Excise small disks about the poles. Since $d(F\eta)=\omega\wedge\eta=0$ off the poles, the outer boundary integral is the sum of the positive small-circle integrals. The latter are $2\pi i\operatorname{res}_p(\eta)F(p)$. Pairing the outer edges as in Solution 1 therefore gives

$$
\sum_i\bigl(A_i(\omega)B_i(\eta)-B_i(\omega)A_i(\eta)\bigr)
=2\pi i\sum_p\operatorname{res}_p(\eta)\int_{p_0}^p\omega.
$$

The paths and the cut polygon are fixed together in this equality. Changing them changes the Abel vector by its [period lattice](../../../../../period-lattice.md), which is precisely the ambiguity we need.

For the sufficiency direction, we need a [differential of the third kind](../../../../../differential-of-the-third-kind.md) with prescribed [residues](../../../../../residue.md) $n_p$. Let $S$ be the reduced support of $D$, consisting of $s$ points. When $s>0$, the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(K_X(S))=g-1+s$. The [residue](../../../../../residue.md) map from this space has [kernel](../../../../../kernel-of-a-linear-map.md) $H^0(K_X)$, of dimension $g$: a differential with at most a simple pole and [residue](../../../../../residue.md) zero has no pole. Its image therefore has dimension $s-1$. The [residue theorem](../../../../../residue-theorem.md) puts the image inside the $s-1$ dimensional space of tuples with sum zero, so it is all that space. In particular there is a [meromorphic differential on a Riemann surface](../../../../../meromorphic-differential-on-a-riemann-surface.md) $\eta$ with [residues](../../../../../residue.md) $n_p$. Subtracting a combination of the normalized [holomorphic one-forms](../../../../../holomorphic-one-form.md) makes all its $a$-periods zero. The bilinear identity then says

$$
(B_1(\eta),\ldots,B_g(\eta))=2\pi i\,u(D),
$$

where on the right we temporarily choose the representative determined by the paths. If $D=0$, we simply take $\eta=0$.

Suppose now that $u(D)=0$ in the [Jacobian variety](../../../../../jacobian-variety.md), so the chosen vector is $m+Bn$, with $m,n\in\mathbb Z^g$. Replace $\eta$ by

$$
\eta'=\eta-2\pi i\sum_jn_j\omega_j.
$$

Its $a$-periods are $-2\pi in_j$ and its $b$-periods are $2\pi im_i$. The periods around the punctures are $2\pi in_p$. These loops together generate the [homology](../../../../../homology-split.md) of the punctured [Riemann surface](../../../../../riemann-surfaces.md), so every period of $\eta'$ lies in $2\pi i\mathbb Z$. Consequently $f(p)=\exp(\int^p\eta')$ is a single-valued nonzero [holomorphic function](../../../../../holomorphic-function.md) off the support of $D$. At a support point, $\eta'=n_p\,dt/t+$ a [holomorphic](../../../../../complex-differentiability-at-a-point.md) differential, so $f=t^{n_p}$ times a nonvanishing [holomorphic function](../../../../../holomorphic-function.md). It extends meromorphically and has [divisor](../../../../../divisor.md) exactly $D$. This proves sufficiency, including negative coefficients.

Conversely, if $D=\operatorname{div}(f)$, take $\eta=df/f$. Its [residues](../../../../../residue.md) are the coefficients of $D$, while its $a$- and $b$-periods are integer multiples of $2\pi i$, by the winding numbers of $f$ along these loops. Writing them as $2\pi ia$ and $2\pi ib$, the [residue](../../../../../residue.md) bilinear identity gives $u(D)=b-Ba\in\Lambda$. Thus $u(D)=0$ in the [Jacobian variety](../../../../../jacobian-variety.md), proving necessity and hence

$$
\boxed{\operatorname{div}(f)=D\text{ for some meromorphic }f\ne0\ \Longleftrightarrow\ \deg D=0\text{ and }u(D)=0.}
$$

Here the displayed necessity of degree zero is also the [residue theorem](../../../../../residue-theorem.md) applied to $df/f$.

There is a useful geometric version of the conclusion. For an effective [divisor](../../../../../divisor.md) $D$, the fiber of $u_d$ through $D$ consists precisely of the effective [divisors](../../../../../divisor.md) [linearly equivalent](../../../../../linear-equivalence-of-weil-divisors.md) to $D$. A nonzero section of $\mathcal O_X(D)$ is a [meromorphic function](../../../../../meromorphic-function.md) $f$ with $\operatorname{div}(f)+D\ge0$, and its zero [divisor](../../../../../divisor.md) as a section is $\operatorname{div}(f)+D$. Two such sections give the same effective [divisor](../../../../../divisor.md) exactly when their ratio is a nonzero constant. Thus the fiber is the [complete linear system of a divisor](../../../../../complete-linear-system-of-a-divisor.md) $|D|=\mathbb P H^0(X,\mathcal O_X(D))$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
