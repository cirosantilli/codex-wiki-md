<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a [closed manifold](../../../../../../closed-manifold.md) $M$ with an oriented [Riemannian metric](../../../../../../riemannian-metric.md), define $\delta$ to be the formal $L^2$ [adjoint operator](../../../../../../adjoint-operator.md) of the [exterior derivative](../../../../../../exterior-derivative.md), equivalently $\delta=(-1)^{n(q+1)+1}*d*$ on $q$-forms. The [Hodge Laplacian](../../../../../../hodge-laplacian.md) is $\Delta_q=d\delta+\delta d$. The [Hodge decomposition theorem](../../../../../../hodge-decomposition-theorem.md) states that its space $\mathcal H^q=\ker\Delta_q$ of [harmonic differential forms](../../../../../../harmonic-differential-form.md) is finite-dimensional and smooth, and that

$$
\boxed{\Omega^q(M)=\mathcal H^q\mathbin{\oplus^\perp}d\Omega^{q-1}(M)\mathbin{\oplus^\perp}\delta\Omega^{q+1}(M),\qquad H^q_{\mathrm{dR}}(M)\cong\mathcal H^q.}
$$

The last isomorphism sends a [harmonic differential form](../../../../../../harmonic-differential-form.md) to its [de Rham cohomology](../../../../../../de-rham-cohomology.md) class: every class has exactly one harmonic representative. Out-of-range degree spaces are zero.

We first justify the analytic facts needed in the proof. In local coordinates and a smooth frame for the form bundle, the [principal symbol](../../../../../../principal-symbol-of-a-partial-differential-equation.md) of $\Delta_q$ is $g^{ij}\xi_i\xi_j I$. This follows from the exterior/contraction identities for $d$ and $\delta$. Freezing the leading coefficients, the [Fourier transform](../../../../../../fourier-transform.md) estimate for the constant positive quadratic form gives, for each nonnegative integer $s$,

$$
\|u\|_{H^{s+2}}\leq C_s\bigl(\|\Delta_q u\|_{H^s}+\|u\|_{L^2}\bigr).
$$

Here is how to pass to variable coefficients. On a sufficiently small coordinate ball the difference of leading coefficients has arbitrarily small supremum norm. After differentiating $s$ times, its top-order contribution is bounded by $\varepsilon\|u\|_{H^{s+2}}$; derivatives of the coefficients and first-order terms contribute $C_s\|u\|_{H^{s+1}}$. A [partition of unity](../../../../../../partition-of-unity.md) gives the same types of terms from commutators with the cutoffs. Absorb the epsilon term and use [Sobolev interpolation](../../../../../../sobolev-interpolation-inequality.md) to absorb $\|u\|_{H^{s+1}}$ into a small multiple of $\|u\|_{H^{s+2}}$ plus $C\|u\|_2$. This proves the estimate.

The first-order energy form $Q(u,u)=\|du\|_2^2+\|\delta u\|_2^2$ satisfies $Q(u,u)+c\|u\|_2^2\geq c'\|u\|_{H^1}^2$ for a sufficiently large $c>0$. This follows from the same frozen-symbol argument at first order, or by integrating the principal part and absorbing the lower-order terms. The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) thus constructs a bounded inverse $R=(\Delta_q+c)^{-1}:L^2\to H^1$ in the weak sense. To obtain $H^2$ regularity of this weak solution, use a local difference quotient $\delta_hu$ and test the weak equation with $-\delta_{-h}(\chi^2\delta_hu)$. Positivity of $g^{ij}$ bounds $\|\chi\delta_h\nabla u\|_2^2$; derivatives of $\chi$ and difference quotients of the smooth coefficients give terms bounded by $C\|u\|_{H^1}\|\chi\delta_h\nabla u\|_2$ and $C\|u\|_{H^1}^2$. The forcing contributes at most $C\|f\|_2(\|\chi\delta_h\nabla u\|_2+\|u\|_{H^1})$. Absorption gives a bound independent of $h$, so the difference-quotient criterion yields $u\in H^2$. Differentiating the equation and repeating gives the higher estimates and smoothness for smooth forcing. Thus the use of [elliptic regularity](../../../../../../elliptic-regularity.md) here has been justified rather than assumed.

The inverse $R$ is compact as an $L^2$ operator by the [Rellich-Kondrachov compactness theorem](../../../../../../rellich-kondrachov-theorem.md), and self-adjoint by symmetry of the weak energy form. It is positive and injective with dense range. The [spectral theorem for compact self-adjoint operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md) now gives an [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) of $\Delta_q$, with nonnegative [eigenvalues](../../../../../../eigenvalue.md) tending to infinity. Each [eigenfunction](../../../../../../eigenfunction.md) is smooth by the estimates above. In particular $\mathcal H^q$ is finite-dimensional and there is a positive gap above its zero [eigenvalue](../../../../../../eigenvalue.md).

Let $H_q$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto $\mathcal H^q$. Define the [Green operator of the Hodge Laplacian](../../../../../../green-operator-of-the-hodge-laplacian.md) by multiplying a positive-eigenvalue coefficient by $1/\lambda$ and sending the zero coefficients to zero. The gap makes this bounded on $L^2$, and the elliptic estimate shows it maps $H^s$ to $H^{s+2}$; hence it sends smooth forms to smooth forms. It obeys

$$
\Delta_qG_q=G_q\Delta_q=I-H_q.
$$

For a smooth $q$-form $\alpha$, expand the left side to obtain

$$
\alpha=H_q\alpha+d\delta G_q\alpha+\delta dG_q\alpha.
$$

These three summands are mutually orthogonal. The energy identity

$$
\langle\Delta_q h,h\rangle=\|dh\|_2^2+\|\delta h\|_2^2
$$

shows that a [harmonic differential form](../../../../../../harmonic-differential-form.md) has both $dh=0$ and $\delta h=0$, making it orthogonal to the exact and coexact summands by [integration by parts](../../../../../../integration-by-parts.md). Also $\langle d\beta,\delta\gamma\rangle=\langle d^2\beta,\gamma\rangle=0$. This proves the claimed direct sum and its uniqueness.

Finally let $d\alpha=0$ and write $u=G_q\alpha$. We have $d\Delta_qu=\Delta_{q+1}du$ because $d^2=0$. Since $d(\alpha-H_q\alpha)=0$, $du$ is harmonic. It is also exact, so its [orthogonality](../../../../../../orthogonal-vectors.md) to harmonic forms gives $du=0$. The decomposition therefore reduces to $\alpha=H_q\alpha+d\delta u$: every [closed differential form](../../../../../../closed-differential-form.md) is cohomologous to a harmonic one. If a harmonic $h$ is exact, $h=d\beta$, then $\|h\|_2^2=\langle\delta h,\beta\rangle=0$. Hence its class is zero only when $h=0$, establishing the isomorphism with [de Rham cohomology](../../../../../../de-rham-cohomology.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
