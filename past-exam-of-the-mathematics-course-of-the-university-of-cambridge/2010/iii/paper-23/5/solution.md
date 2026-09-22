<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [one-variable main conjecture for CM elliptic curves](../../../../../one-variable-main-conjecture-for-cm-elliptic-curves.md) compares a torsion arithmetic [Iwasawa module](../../../../../iwasawa-module.md) with a measure interpolating special [Hecke L-function](../../../../../hecke-l-function.md) values. The classical bounded-measure formulation uses a prime of [good reduction](../../../../../good-reduction-of-an-elliptic-curve.md) which splits in the CM field, hence gives [ordinary reduction](../../../../../ordinary-reduction-of-an-elliptic-curve.md). We first describe the one-prime division-tower formulation, including the analytic construction, and then explain its cyclotomic Selmer counterpart and the change at supersingular primes.

For a precise basic setting, take $E/K$ with [complex multiplication](../../../../../complex-multiplication.md) by $\mathcal O_K$, $K$ of class number one, and a split prime $p>3$ of [good reduction](../../../../../good-reduction-of-an-elliptic-curve.md), prime to the Hecke conductor $\mathfrak f$. Write $p\mathcal O_K=\mathfrak p\bar{\mathfrak p}$, choose the $p$-adic embedding corresponding to $\mathfrak p$, and let $\pi=\psi_E(\mathfrak p)$. Its [formal group of an elliptic curve](../../../../../formal-group-of-an-elliptic-curve.md) has height one, with $[\pi](t)\equiv t^p\pmod{\mathfrak p}$. The one-prime division tower

$$
F_\infty=K(E[\mathfrak p^\infty]),\qquad G=\operatorname{Gal}(F_\infty/K)=\Delta\times\Gamma
$$

has $\Delta$ of order prime to $p$ and $\Gamma\simeq\mathbb Z_p$. Its CM character $\kappa:G\to\mathbb Z_p^\times$ describes the action on the prime-primary [Tate module](../../../../../tate-module.md). Let $F=F_\infty^\Gamma$ and $\Lambda=I[[\Gamma]]\simeq I[[T]]$. We extend coefficients to the complete unramified [ring](../../../../../ring.md) $I$ to include character values and a [CM period](../../../../../cm-period.md).

Let $X$ be the [Galois group](../../../../../galois-group.md) over $F_\infty$ of the maximal abelian pro-$p$ extension unramified outside primes above $\mathfrak p$. Let $A$ be the analogous everywhere-unramified group, equivalently the norm inverse limit of the $p$-parts of the ideal class groups. Write $U$ for the norm limit of principal local units at $\mathfrak p$, $\mathcal E$ for the closures of global units in $U$, and $\mathcal C$ for the closures of [elliptic units](../../../../../elliptic-unit.md). Roots of unity and finite initial-layer errors are retained when formulating integral statements; after passage to a finite-character component they do not change a [characteristic ideal](../../../../../characteristic-ideal.md).

The [class-field unit sequence](../../../../../class-field-unit-sequence.md), obtained by taking norm limits in global [Artin reciprocity](../../../../../artin-reciprocity-law.md), gives

$$
0\longrightarrow\mathcal E/\mathcal C\longrightarrow U/\mathcal C\longrightarrow X\longrightarrow A\longrightarrow0.
$$

In this ordinary one-prime tower, the unit and global-unit terms have the same Iwasawa rank, and the displayed quotients and $X,A$ are torsion on their character components. The equality

$$
\operatorname{char}_\Lambda(\mathcal E/\mathcal C)_\chi=\operatorname{char}_\Lambda A_\chi
$$

is the global-units/class-groups form of the CM main theorem. Multiplicativity of [characteristic ideals](../../../../../characteristic-ideal.md) in the sequence then gives

$$
\operatorname{char}_\Lambda X_\chi=\operatorname{char}_\Lambda(U/\mathcal C)_\chi.
$$

The analytic construction must identify the latter ideal with a genuinely interpolating [p-adic L-function](../../../../../p-adic-l-function.md); it is not enough to rename an arbitrary characteristic power series as an L-function.

Here is that construction. For an auxiliary ideal $\mathfrak a$ prime to $6p\mathfrak f$, a suitably normalized rational elliptic function has divisor a multiple of

$$
N\mathfrak a\,(O)-\sum_{P\in E[\mathfrak a]}(P).
$$

Translate by a generator of the conductor torsion and take the product over its ray-class orbit. This produces a rational function $f_\mathfrak a(t)$ defined over $K$ which is a unit series at the identity. Evaluating it on compatible $\mathfrak p^n$-division points gives [elliptic units](../../../../../elliptic-unit.md). The reason for the norm relations is geometric: multiplication by $\pi$ groups the translated zeros and poles into fibers, so the product over $E[\mathfrak p]$ has the divisor of $f_\mathfrak a([\pi]t)$. The normalization fixes the constant, giving the local identity

$$
\prod_{Q\in E[\mathfrak p]}f_\mathfrak a(t+_{\widehat E}Q)=f_\mathfrak a([\pi]t).
$$

This is also the norm relation of the [Coleman power series for a CM formal group](../../../../../coleman-power-series-for-a-cm-formal-group.md) interpolating the resulting local units.

An integral logarithmic correction makes the passage from those units to a bounded measure explicit. In the chosen split completion $K_\mathfrak p=\mathbb Q_p$, put

$$
\mathcal L_f(t)=\log f(t)-\frac1p\log f([\pi]t)=\frac1p\log\frac{f(t)^p}{f([\pi]t)}.
$$

Since $[\pi]t\equiv t^p\pmod p$ and the coefficients of $f$ reduce to $\mathbb F_p$, the ratio is in $1+p\mathbb Z_p[[t]]$. For $p>2$, its logarithm divided by $p$ is integral. Constants are treated using the usual $p$-adic logarithm on units. This proves the integrality needed for the [Frobenius-corrected logarithm](../../../../../frobenius-corrected-logarithm.md); applying an uncorrected logarithm alone would not prove boundedness.

Choose an isomorphism $\eta:\widehat{\mathbb G}_m\to\widehat E$ over $I$, and normalize the [CM period](../../../../../cm-period.md) by

$$
\log_{\widehat E}(\eta(T))=\Omega_p\log(1+T).
$$

Then $A_f(T)=\mathcal L_f(\eta(T))\in I[[T]]$ is the [Amice transform](../../../../../amice-transform.md) of a unique $I$-valued [p-adic measure](../../../../../p-adic-measure.md) on $\mathbb Z_p$. The norm relation above gives

$$
\sum_{\zeta^p=1}A_f(\zeta(1+T)-1)=0:
$$

the first logarithmic sum is $\log f([\pi]t)$ and the second is the same sum, because $[\pi]Q=0$ and there are $p$ points. On the measure side the sum selects $p\mathbb Z_p$ and multiplies by $p$, so this identity says that the measure is supported on $\mathbb Z_p^\times$. Transport it to $G$ by the CM character and project to the desired component.

The moments can now be calculated rather than postulated. With $D=(1+T)d/dT$,

$$
\int x^k\,d\mu_f(x)=D^kA_f(0)=\Omega_p^k\left(1-\frac{\pi^k}{p}\right)\left.\frac{d^k}{dz^k}\log f(\exp_{\widehat E}z)\right|_{z=0}\quad(k\geq1).
$$

The factor $\pi^k$ appears because $[\pi]$ is multiplication by $\pi$ in the additive formal-logarithm coordinate. The remaining derivative is a [Coates–Wiles homomorphism](../../../../../coates-wiles-homomorphism.md). The complex product for the elliptic function makes it a sum of shifted inverse powers of lattice elements. Grouping these lattice elements by ray-class ideals identifies that sum with $(k-1)!L_{\mathfrak f}(\bar\psi_E^{\,k},k)/\Omega_\infty^k$, multiplied by the auxiliary factor $N\mathfrak a-\psi_E(\mathfrak a)^k$. Here $L_{\mathfrak f}$ omits primes dividing the original conductor, including when the conductor of the power character becomes smaller.

Normalize the rational functions and matching complex and $p$-adic periods consistently, and remove the auxiliary factors by the distribution relations. They are evaluations of $N\mathfrak a-[\mathfrak a]$ in the [Iwasawa algebra](../../../../../iwasawa-algebra.md). On each finite-character component an auxiliary ideal can be chosen making this element a unit: its residues at $\mathfrak p$ and $\bar{\mathfrak p}$ can be prescribed independently by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md). The resulting integral measure $\mu_E$ satisfies, on its branch and with $k$ in the corresponding residue class,

$$
\boxed{\Omega_p^{-k}\int_G\kappa(g)^k\,d\mu_E(g)=(k-1)!\left(1-\frac{\psi_E(\mathfrak p)^k}{p}\right)\frac{L_{\mathfrak f}(\bar\psi_E^{\,k},k)}{\Omega_\infty^k}.}
$$

The exact normalization of periods matters for this equality; multiplication by an integral unit does not affect the ideal in the main conjecture. Finite-order twists are obtained by inserting a character in the ray-class sums, with its local Gauss sum. The lattice calculation proves algebraicity of the normalized complex values, while the integral series construction proves their $p$-adic interpolation. These are different steps.

The Coleman measure map identifies $U_\chi$ with a rank-one [Iwasawa algebra](../../../../../iwasawa-algebra.md) lattice, up to finite errors, and takes $\mathcal C_\chi$ to the ideal generated by the corresponding power series $\mathcal L_\chi$. The conjecture therefore has the concrete form

$$
\boxed{\operatorname{char}_{I[[\Gamma]]}X_\chi=(\mathcal L_\chi).}
$$

Its proof uses the [Euler system of elliptic units](../../../../../euler-system-of-elliptic-units.md). Adjoining auxiliary ray moduli supplies norm relations with factors $1-\operatorname{Frob}_{\mathfrak q}^{-1}$. Derivative operators in the auxiliary cyclic groups produce Kolyvagin classes; their controlled valuations relate a new auxiliary prime to its ideal class. [Chebotarev density theorem](../../../../../chebotarev-density-theorem.md) permits the required Frobenius choices. Successively choosing these primes bounds the class-group elementary divisors by the elliptic-unit index, giving the difficult characteristic-ideal divisibility. The opposite comparison comes from the class-number/unit-index formula and passage through the tower. Their equality, combined with the exact sequence above and the logarithmic computation, is the proof mechanism. The ordinary split-prime setting of this formulation is specified in [Rubin's one-variable main-conjecture paper](https://www.cambridge.org/core/books/abs/lfunctions-and-arithmetic/onevariable-main-conjecture-for-elliptic-curves-with-complex-multiplication/58848581663E1D54A747951F3034421F).

For completeness, the familiar cyclotomic formulation concerns a different tower. If $E/\mathbb Q$ has [complex multiplication](../../../../../complex-multiplication.md) and good ordinary reduction at $p$, put $\Gamma_{\rm cyc}=\operatorname{Gal}(\mathbb Q_\infty/\mathbb Q)$ and

$$
\mathcal X_E=\operatorname{Hom}_{\rm cont}(\operatorname{Sel}_{p^\infty}(E/\mathbb Q_\infty),\mathbb Q_p/\mathbb Z_p).
$$

For a finite layer $L$, its [Selmer group of an elliptic curve](../../../../../n-selmer-group.md) is

$$
\ker\left(H^1(G_S(L),E[p^\infty])\longrightarrow\prod_{v\in S}\frac{H^1(L_v,E[p^\infty])}{\operatorname{im}(E(L_v)\otimes\mathbb Q_p/\mathbb Z_p)}\right),
$$

where $S$ contains the bad primes and primes above $p$; at infinite level take the direct limit. Thus it imposes the local Kummer conditions and sits between rational points tensored with $\mathbb Q_p/\mathbb Z_p$ and the $p$-primary [Tate–Shafarevich group](../../../../../tate-shafarevich-group.md). Its dual $\mathcal X_E$ is a torsion [Iwasawa module](../../../../../iwasawa-module.md), and the cyclotomic main conjecture is

$$
\boxed{\operatorname{char}_{\mathbb Z_p[[\Gamma_{\rm cyc}]]}\mathcal X_E=(L_p(E)).}
$$

With compatible reciprocity conventions, the ordinary function has the finite-character interpolation

$$
\chi(L_p(E))=\alpha^{-n}\tau(\chi)\frac{L(E,\bar\chi,1)}{\Omega_E^+}\quad(\operatorname{cond}\chi=p^n>1),\qquad L_p(E)(1)=(1-\alpha^{-1})^2\frac{L(E,1)}{\Omega_E^+},
$$

where $\alpha$ is the $p$-adic unit root of $X^2-a_pX+p$ and $\tau(\chi)=\sum_{a\bmod p^n}\chi(a)e^{2\pi ia/p^n}$; characters of this cyclotomic $\mathbb Z_p$-extension are even. The two-variable CM measure specializes to this line after the CM-character twist. [Kummer theory](../../../../../kummer-theory.md), class-field descriptions of the prime-primary local conditions and control of finite-layer errors identify its algebraic counterpart with the displayed Selmer dual. The one-prime division tower is not itself the cyclotomic tower, so this requires the twist and specialization argument, not just changing its name.

Finally, at a good inert prime the curve has [supersingular reduction](../../../../../supersingular-reduction-of-an-elliptic-curve.md). The ordinary unit root is absent, the unmodified cyclotomic Selmer dual is not torsion, and the ordinary bounded-function argument does not apply. For CM curves over $\mathbb Q$ and odd supersingular $p$, signed local trace conditions and signed functions give instead $\operatorname{char}\mathcal X_E^\pm=(L_p^\pm(E))$, as proved in [Pollack and Rubin's supersingular main-conjecture theorem](https://math.arizona.edu/~rpollack/Papers/Main_conjecture_for_CM_elliptic_curves_at_ss_primes.pdf). Thus the ordinary hypotheses and the analytic local correction are essential parts of the essay's main-conjecture statement.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
