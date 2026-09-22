<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The gauge-invariant [Yang-Mills action](../../../../../yang-mills-action.md) integrates over physically equivalent configurations along each [gauge orbit](../../../../../gauge-orbit.md). At the quadratic level its gauge-field kernel has longitudinal zero directions: in [momentum](../../../../../momentum.md) space $K_{\mu\nu}(k)=-k^2\eta_{\mu\nu}+k_\mu k_\nu$ satisfies $K_{\mu\nu}k^\nu=0$. It therefore has no inverse from which to construct a [gauge-boson propagator](../../../../../gauge-boson-propagator.md). [Gauge fixing](../../../../../gauge-fixing.md) both removes the redundant orbit integration and supplies an invertible quadratic operator away from the ordinary physical propagator poles.

For the covariant condition $\partial^\mu A_\mu=0$, the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) is that of $\partial^\mu D_\mu$. Its representation by odd [Faddeev-Popov ghost fields](../../../../../faddeev-popov-ghost.md) and [antighost fields](../../../../../faddeev-popov-antighost-field.md) produces the displayed ghost term. In a nonabelian theory $D_\mu$ depends on the [gauge field](../../../../../gauge-field.md), so the [determinant](../../../../../determinant.md) is not an irrelevant constant: ghost interactions must be retained. The even [Nakanishi-Lautrup field](../../../../../nakanishi-lautrup-field.md) $b$ writes [gauge fixing](../../../../../gauge-fixing.md) in a form with off-shell [BRS symmetry](../../../../../brst-symmetry.md). For $\xi\ne0$, its algebraic equation is $b=-\partial\cdot A/\xi$, giving $-(\partial\cdot A)^2/(2\xi)$ after elimination. At $\xi=0$ it imposes the gauge condition as a [Lagrange multiplier](../../../../../lagrange-multiplier.md).

For the nilpotence proof, write the adjoint bracket as $[X,Y]^a=f^{abc}X^bY^c$, with coefficients in a [Grassmann algebra](../../../../../grassmann-algebra.md). If $|X|,|Y|$ are their parities, this is a [graded Lie bracket](../../../../../graded-lie-bracket.md):

$$
[X,Y]=-(-1)^{|X||Y|}[Y,X].
$$

Thus two odd fields have a symmetric bracket, in particular $[c,c]$ need not vanish. The transformations become $sA_\mu=D_\mu c$, $sc=-[c,c]/2$, $s\bar c=-b$, $sb=0$, and $s$ obeys the left [graded Leibniz rule](../../../../../graded-leibniz-rule.md).

Because $D_\mu$ is even, $D_\mu[c,c]=[D_\mu c,c]+[c,D_\mu c]=2[D_\mu c,c]$. Varying both the field and the connection in $D_\mu c$ now gives

$$
s^2A_\mu=s(D_\mu c)=D_\mu(sc)+[sA_\mu,c]
=-\frac12D_\mu[c,c]+[D_\mu c,c]=0.
$$

For the ghost,

$$
s^2c=-\frac12\{[sc,c]-[c,sc]\}
=-[sc,c]=\frac12[[c,c],c]=0.
$$

The last equality is the [graded Jacobi identity](../../../../../graded-jacobi-identity.md) applied to three copies of the odd field $c$. In components the remaining expression is $\tfrac12 f^{abc}f^{bde}c^dc^ec^c$; its coefficient is antisymmetrized over $c,d,e$, and the ordinary [Jacobi identity](../../../../../jacobi-identity.md) for the structure constants makes that antisymmetrization zero. Finally $s^2\bar c=-sb=0$ and $s^2b=0$. Hence

$$
\boxed{s^2=0\quad\text{on all four fields, without field equations}.}
$$

This is [off-shell nilpotence of the Yang-Mills BRST quartet](../../../../../off-shell-nilpotence-of-the-yang-mills-brst-quartet.md).

To verify invariance of the complete Lagrangian, $sF_{\mu\nu}=[F_{\mu\nu},c]$, obtained from $[D_\mu,D_\nu]c=[F_{\mu\nu},c]$. Thus $s(F_{\mu\nu}^aF^{\mu\nu a})=0$ because the product of the two curvature components is symmetric in their color labels while $f^{abc}$ is antisymmetric. The remaining terms vary as

$$
\begin{aligned}
s(b^a\partial^\mu A_\mu^a)&=b^a\partial^\mu(D_\mu c)^a,\\
s(\xi b^ab^a/2)&=0,\\
s(\bar c^a\partial^\mu(D_\mu c)^a)&=-b^a\partial^\mu(D_\mu c)^a-\bar c^a\partial^\mu s(D_\mu c)^a.
\end{aligned}
$$

The last term vanishes by the already proved $s^2A=0$, and the first and third terms cancel pointwise. Therefore

$$
\boxed{s\mathcal L=0.}
$$

Equivalently, the [covariant gauge-fixing density as a BRST variation](../../../../../covariant-gauge-fixing-density-as-a-brst-variation.md) is $s\Psi$ with $\Psi=-\bar c^a(\partial\cdot A^a+\xi b^a/2)$. The graded sign from moving $s$ past $\bar c$ produces the positive ghost term, and $s^2\Psi=0$ proves its invariance. No integration-by-parts qualification is needed for the density as written.

Let $Q=Q_{\mathrm{BRS}}$ be the [BRS charge](../../../../../brst-charge.md). The physical state space is its [BRST cohomology](../../../../../brst-cohomology.md), usually at [ghost number](../../../../../ghost-number.md) zero:

$$
\boxed{\mathcal H_{\rm phys}=\ker Q/\operatorname{im}Q.}
$$

Nilpotence ensures $\operatorname{im}Q\subseteq\ker Q$. A state $Q|\chi\rangle$ is orthogonal to every closed state because $\langle\psi|Q|\chi\rangle=\langle Q\psi|\chi\rangle=0$, and its norm is $\langle\chi|Q^2|\chi\rangle=0$. Thus adding an exact state changes neither physical inner products nor amplitudes. Self-adjointness here is relative to the stated indefinite [Hermitian form](../../../../../hermitian-form.md); a nonzero self-adjoint [nilpotent operator](../../../../../nilpotent-linear-map.md) could not exist on a positive-definite state space. Positivity must be proved on the quotient, not assumed on the gauge/ghost space.

Fix a color label and a nonzero [momentum](../../../../../momentum.md) $k$, and take the usual nontrivial asymptotic charge, $\alpha\ne0$. Nilpotence on a vector state gives $Q|c\rangle=0$, because at least one component of $k$ is nonzero. Nilpotence on the antighost state then gives

$$
0=Q^2|\bar c\rangle=\bar\alpha\alpha k^\mu k_\mu|c\rangle,
\qquad\boxed{k^2=0.}
$$

The two coefficients are complex conjugates as required by self-adjointness: using the given ghost pairing,

$$
\langle A_\nu|Q|\bar c\rangle=\bar\alpha k_\nu
=\langle QA_\nu|\bar c\rangle=\alpha^*k_\nu.
$$

Thus the antighost-to-vector coefficient is $\alpha^*$, as the printed bar notation indicates. These conditions are the massless shell condition and the consistency of the charge with the inner products.

A general one-particle vector representative is $|\varepsilon\rangle=\varepsilon^\mu|A_\mu\rangle$. It is closed precisely when $k_\mu\varepsilon^\mu=0$. The vector state $k^\mu|A_\mu\rangle=Q|\bar c\rangle/\bar\alpha$ is exact, so representatives obey

$$
\varepsilon\sim\varepsilon+zk.
$$

The ghost state is also exact: choose $v^\mu$ with $\alpha v\cdot k=1$, then $Q(v^\mu|A_\mu\rangle)=|c\rangle$. The antighost state is not closed because its image is a nonzero longitudinal vector. More explicitly, closure of a general sum of vector, ghost and antighost states forces the antighost coefficient to vanish and the vector polarization to be orthogonal to $k$; its ghost component disappears in the quotient. Thus the full one-particle cohomology already reduces to

$$
\boxed{\{\varepsilon:k\cdot\varepsilon=0\}/\operatorname{span}\{k\}.}
$$

With the mostly-plus [Minkowski metric](../../../../../minkowski-metric.md), choose a Lorentz frame with $k^\mu=(\omega,0,0,\omega)$, $\omega>0$. Closure gives $\varepsilon^3=\varepsilon^0$, and the norm is

$$
\langle\varepsilon|\varepsilon\rangle
=-|\varepsilon^0|^2+|\varepsilon^1|^2+|\varepsilon^2|^2+|\varepsilon^3|^2
=|\varepsilon^1|^2+|\varepsilon^2|^2.
$$

Subtracting a multiple of $k$ sets $\varepsilon^0=\varepsilon^3=0$. Consequently [positive one-particle BRST cohomology](../../../../../positive-one-particle-brst-cohomology.md) consists of **two transverse positive-norm polarizations per color**, represented by $|A_1\rangle,|A_2\rangle$. A nonzero class has strictly positive norm; the zero-norm longitudinal direction was precisely the exact direction removed.

The qualifications $k\ne0$ and $\alpha\ne0$ are essential to this one-particle argument. The zero-momentum sector requires separate treatment, and the trivial-charge case cannot yield the asserted removal of negative-norm vector states from the stated relations alone. Abstract nilpotence and self-adjointness by themselves do not guarantee positive cohomology.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
