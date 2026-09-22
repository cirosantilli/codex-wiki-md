<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Gaussian free field](../../../../../gaussian-free-field.md) is a random distribution, so its purported level curve cannot be defined by evaluating its height at every point. A coupling must instead be stated using conditional means and covariances. The [SLE4 coupling with a Gaussian free field](../../../../../sle4-coupling-with-a-gaussian-free-field.md) does exactly this.

Choose the Green-function normalization

$$
G_{\mathbb H}(z,w)=\log\left|\frac{z-\overline w}{z-w}\right|,
\qquad -\Delta_zG_{\mathbb H}(z,w)=2\pi\delta_w(z).
$$

A [Zero-boundary Gaussian free field](../../../../../zero-boundary-gaussian-free-field.md) $H_0$ is characterized on real compactly supported smooth [test functions](../../../../../test-function.md) by

$$
\mathbb E(H_0,\varphi)=0,\qquad
\operatorname{Cov}((H_0,\varphi),(H_0,\psi))
=\iint\varphi(z)G_{\mathbb H}(z,w)\psi(w)\,dA(z)dA(w).
$$

Equivalently its energy normalization is the [Dirichlet inner product](../../../../../dirichlet-inner-product.md) $(2\pi)^{-1}\int\nabla f\cdot\nabla g\,dA$. This fixes the otherwise convention-dependent height constant.

Set $\lambda=\pi/2$ and

$$
m_0(z)=\lambda-\frac{2\lambda}{\pi}\arg z,
\qquad H=H_0+m_0.
$$

The field $H$ has prescribed Dirichlet values $-\lambda$ on the negative half-line and $+\lambda$ on the positive half-line. Subtracting $m_0$ recovers the zero-Dirichlet field $H_0$. It is the shifted field $H$, rather than an unshifted zero-boundary field, whose zero-height interface has ordinary chordal $\operatorname{SLE}_4$ law.

Let $\eta$ be chordal $\operatorname{SLE}_4$ from $0$ to $\infty$, with [Chordal Loewner equation](../../../../../chordal-loewner-equation.md) $\partial_tg_t=2/(g_t-W_t)$ and $W_t=2\beta_t$. Write $D_t=\mathbb H\setminus\eta[0,t]$ and $f_t=g_t-W_t$. The coupling statement is:

$$
\boxed{\mathcal L(H\mid\eta[0,t])=
\mathcal L\bigl(H^{D_t}_0+m_t\bigr),\qquad
m_t(z)=\lambda-\frac{2\lambda}{\pi}\arg f_t(z),}
$$

where, conditionally on the curve, $H^{D_t}_0$ is an independent zero-boundary field in the slit domain. The equality is for restrictions to [test functions](../../../../../test-function.md) in that domain, and extends to suitable stopping times. Its [covariance](../../../../../covariance.md) is $G_{D_t}(z,w)=G_{\mathbb H}(f_t(z),f_t(w))$ by conformal invariance. The two sides of the revealed slit have heights $-\lambda$ and $+\lambda$, in the order specified by their real images under $f_t$. This is the continuum meaning of a [Gaussian free field level line](../../../../../gaussian-free-field-level-line.md).

The fundamental calculations explain why the parameter is four. For $Z_t=f_t(z)$, the [Itô formula](../../../../../ito-s-lemma.md) gives

$$
d\log Z_t=\frac{2-\kappa/2}{Z_t^2}\,dt
-\frac{\sqrt\kappa}{Z_t}\,d\beta_t.
$$

At $\kappa=4$ the drift vanishes. Thus

$$
dm_t(z)=\frac{4\lambda}{\pi}\operatorname{Im}\frac1{f_t(z)}\,d\beta_t
=2\operatorname{Im}\frac1{f_t(z)}\,d\beta_t.
$$

Each harmonic mean is a bounded [martingale](../../../../../martingale-split.md) before approaching its point. Differentiating the explicit conformally transformed Green function gives the [Loewner variation of the Dirichlet Green function](../../../../../loewner-variation-of-the-dirichlet-green-function.md)

$$
\frac d{dt}G_{D_t}(z,w)
=-4\operatorname{Im}\frac1{f_t(z)}\operatorname{Im}\frac1{f_t(w)}.
$$

Therefore

$$
\boxed{d\langle m(z),m(w)\rangle_t=-dG_{D_t}(z,w).}
$$

In words, the variance learned from the evolving mean exactly equals the [covariance](../../../../../covariance.md) lost when the slit is removed. For a Green kernel $cG$ the same calculation gives $\lambda=(\pi/2)\sqrt c$; using a different Green normalization changes the height constant, not the [SLE](../../../../../schramm-loewner-evolution.md) parameter.

To construct the coupling, first sample the [SLE](../../../../../schramm-loewner-evolution.md) curve. In the two components to its left and right, sample independent zero-boundary fields and add the corresponding constant heights. Extend these as distributions to obtain the candidate full field. The following [martingale](../../../../../martingale-split.md) identity proves its marginal law rather than merely matching its first two moments.

For a real [test function](../../../../../test-function.md) $\varphi$, put $M_t=(m_t,\varphi)$ and

$$
V_t=\iint\varphi(z)G_{D_t}(z,w)\varphi(w)\,dA(z)dA(w).
$$

Localization permits integration of the pointwise identities. They yield $d\langle M\rangle_t=-dV_t$. Hence

$$
\mathcal Z_t=\exp\left(iM_t-\frac12V_t\right)
$$

is a complex [local martingale](../../../../../local-martingale.md): the $-\tfrac12dV_t$ drift cancels the $-\tfrac12d\langle M\rangle_t$ Itô correction. Since $V_t\geq0$, $|\mathcal Z_t|\leq1$, making it a true [martingale](../../../../../martingale-split.md). At the complete-curve limit, $m_t$ becomes the constant height in each component and the remaining Green kernel becomes that of those components. Thus $\mathcal Z_\infty$ is the conditional [characteristic function](../../../../../characteristic-function.md) of the sampled candidate field. Taking expectations gives

$$
\mathbb E\mathcal Z_\infty
=\exp\left(i(m_0,\varphi)-\frac12\iint\varphi G_{\mathbb H}\varphi\right).
$$

Applying this to every linear combination of [test functions](../../../../../test-function.md) proves the entire Gaussian law, not only its [covariance](../../../../../covariance.md). The conditional version $\mathbb E(\mathcal Z_\infty\mid\mathcal F_t)=\mathcal Z_t$ proves the displayed conditional-field statement. Exhaustion by compact test supports justifies passage across the slit and the limiting distributional extensions.

This revealed curve is a [local set of a Gaussian free field](../../../../../local-set-of-a-gaussian-free-field.md): conditionally on it, the remaining field is a zero-boundary field plus a specified [harmonic function](../../../../../harmonic-function.md). The spatial Markov property is thereby preserved at random domains, a property not available for arbitrary field-dependent sets. One can strengthen the coupling to a curve measurable from the field. The proof explores compatible interfaces in small subdomains and uses the conditional boundary heights and monotonicity to show that two such interfaces for the same field cannot separate; a countable exhaustion gives uniqueness. This supplies a rigorous replacement for the informal phrase “draw the zero contour.” It does not assert that the distribution has pointwise values.

The coupling is useful in both directions: [SLE](../../../../../schramm-loewner-evolution.md) [martingales](../../../../../martingale-split.md) give exact conditional [Gaussian free field](../../../../../gaussian-free-field.md) data, while the Gaussian Markov structure explains the [SLE](../../../../../schramm-loewner-evolution.md) domain Markov property and its distinguished parameter. **With the above normalization, the height jump is $2\lambda=\pi$, and the corresponding interface is [chordal SLE4](../../../../../chordal-sle4.md).**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
