<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take a positive [gradient](../../../../../gradient.md) coefficient $\kappa^{-1}$, a positive squared mass, a finite-volume regulator and an [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md). Use the dimensionless statistical action convention $Z=\int\mathcal D\phi\,e^{-H}$: inverse temperature is absorbed into the coefficients. If $H$ denotes dimensional energy instead, the exponent below gains a factor $\beta_{\rm th}$ and the covariance gains $\beta_{\rm th}^{-1}$. These conventions cannot be mixed.

Choose the [Fourier transform](../../../../../fourier-transform.md) convention

$$
\phi(x)=\int\frac{d^Dp}{(2\pi)^D}e^{ip\cdot x}\widetilde\phi(p),\qquad\widetilde\phi(-p)=\widetilde\phi(p)^*.
$$

Integration of the quadratic [gradient](../../../../../gradient.md) and source terms gives

$$
H=\frac12\int\frac{d^Dp}{(2\pi)^D}\widetilde\phi(p)\widetilde\Delta(p)\widetilde\phi(-p)-\int\frac{d^Dp}{(2\pi)^D}\widetilde J(p)\widetilde\phi(-p),\qquad\boxed{\widetilde\Delta(p)=\kappa^{-1}p^2+m^2.}
$$

Complete the square with $\widetilde\phi_{\rm cl}(p)=\widetilde\Delta(p)^{-1}\widetilde J(p)$. Translation of the regulated real Gaussian variables leaves their measure unchanged, so the [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
\boxed{Z_0[J]=Z_G\exp\left[\frac12\int\frac{d^Dp}{(2\pi)^D}\widetilde J(p)\widetilde\Delta(p)^{-1}\widetilde J(-p)\right].}
$$

Here $Z_G=Z_0[0]$ is the source-free Gaussian [partition function](../../../../../canonical-partition-function.md). For $n$ independent regulated real coordinates and a positive quadratic matrix $A$, it is $(2\pi)^{n/2}(\det A)^{-1/2}$ under Lebesgue normalization. The continuum [determinant](../../../../../determinant.md) needs the stated regulator and a measure convention. Reality pairs the nonzero Fourier modes, so they must not be counted as two independent real fields.

A [connected correlation function](../../../../../connected-correlation-function.md) subtracts the product of the means. The logarithm $W[J]=\log Z_0[J]$ generates its cumulants: differentiating $W$ twice with respect to the source, using the measure $d^Dp/(2\pi)^D$ in the [functional derivative](../../../../../functional-derivative.md) convention, yields

$$
\langle\widetilde\phi(p)\rangle=\frac{\widetilde J(p)}{\widetilde\Delta(p)},\qquad\boxed{\langle\widetilde\phi(q)\widetilde\phi(p)\rangle_c=(2\pi)^D\delta^{(D)}(p+q)\widetilde G_0(p),\quad\widetilde G_0(p)=\frac1{\kappa^{-1}p^2+m^2}.}
$$

The source changes the mean but not the covariance; the stated zero-source limit therefore follows immediately. Momentum conservation uses $p+q$, appropriate for a real field without complex conjugation on either displayed factor.

For the continuum [massive Gaussian field correlation tail](../../../../../massive-gaussian-field-correlation-tail.md), set $\mu=\sqrt\kappa\,m>0$ and $r=|x|$. Fourier inversion gives

$$
G_0(r)=\frac{\kappa}{(2\pi)^{D/2}}\left(\frac\mu r\right)^{D/2-1}K_{D/2-1}(\mu r).
$$

The large-argument [Modified Bessel function of the second kind](../../../../../modified-bessel-function-of-the-second-kind.md) has $K_\rho(z)\sim\sqrt{\pi/(2z)}e^{-z}$. Hence $G_0(r)$ is proportional to $r^{-(D-1)/2}e^{-\mu r}$ at large distance and

$$
\boxed{\xi=\frac1{\sqrt\kappa\,m}\propto\frac1m\quad\text{for fixed positive }\kappa.}
$$

At zero mass the exponential length diverges. For $D>2$ the critical continuum tail is algebraic, $G_0(r)\propto r^{2-D}$; in lower dimensions infrared regulation needs additional care.

For a uniform source $h$, perform a [momentum-shell renormalization group](../../../../../momentum-shell-renormalization-group.md) step: separate slow modes $|p|<\Lambda/b$ and fast modes $\Lambda/b<|p|<\Lambda$. In a [Gaussian field theory](../../../../../gaussian-field-theory.md) they decouple; the uniform source couples only to the retained zero mode. Integrating fast modes contributes only a field-independent [determinant](../../../../../determinant.md) to the [free energy](../../../../../thermodynamic-free-energy.md). Restore the cutoff by $x'=x/b$, $p'=bp$ and

$$
\phi'(x')=b^{(D-2)/2}\phi_<(bx').
$$

The factors from the measure, [gradient](../../../../../gradient.md) and two fields cancel in the [gradient](../../../../../gradient.md) term. The mass term gains $b^2$, and the linear source gains $b^{(D+2)/2}$. Therefore

$$
\boxed{\kappa'=\kappa,\qquad(m')^2=b^2m^2,\quad m'=bm,\qquad h'=b^{(D+2)/2}h.}
$$

Here $m$ is the positive mass; for signed thermal coordinates it is the squared-mass relation that applies. The [Gaussian fixed point](../../../../../gaussian-fixed-point.md) has thermal scaling eigenvalue $\lambda_t=2$, source eigenvalue $\lambda_h=(D+2)/2$ and zero anomalous dimension.

Under the formal homogeneous Gaussian scaling hypothesis, substitution of those eigenvalues gives

$$
\boxed{\alpha=\frac{4-D}{2},\qquad\beta=\frac{D-2}{4},\qquad\nu=\frac12,\qquad\gamma=1\quad(D<4).}
$$

The last two values are independently visible in $\xi\propto t^{-1/2}$ and $\chi=\widetilde G_0(0)=1/m^2\propto t^{-1}$, agreeing with [Landau-Ginzburg theory](../../../../../landau-ginzburg-theory.md). The specific-heat power follows directly from the [determinant](../../../../../determinant.md): after two thermal derivatives its singular contribution is proportional to

$$
\int_{|p|<\Lambda}\frac{d^Dp}{(2\pi)^D}\frac1{(\kappa^{-1}p^2+t)^2}\propto t^{D/2-2}\quad(0<D<4).
$$

The change of variables $p=\sqrt{\kappa t}\,q$ proves this power because the rescaled integral converges at large $q$ exactly when $D<4$. The two-dimensional [free energy](../../../../../thermodynamic-free-energy.md) itself has a $t\log t$ resonance, while its second derivative still has the indicated $t^{-1}$ power.

**The printed [magnetization](../../../../../magnetization.md) exponent is a formal Gaussian scaling index, not a proved ordered-phase law of the purely quadratic model.** The [ordered-phase obstruction in a Gaussian scalar model](../../../../../ordered-phase-obstruction-in-a-gaussian-scalar-model.md) is explicit: the uniform field has energy density $m^2M^2/2-hM$. At $h=0,m^2<0$ it tends to $-\infty$ as $|M|\to\infty$, and the [partition function](../../../../../canonical-partition-function.md) diverges. For $m^2>0$, the mean is $M=h/m^2$ and tends to zero as $h\to0$, so there is no spontaneously ordered branch. Thus no literal $M\sim|t|^\beta$ for $t<0$ can be established from this [Statistical Hamiltonian](../../../../../statistical-hamiltonian.md) alone. The value $(D-2)/4$ follows from the scaling dimension of the field if one assumes such a branch; for $D\leq2$ its nonpositive value further warns against that interpretation. Adding a stabilizing quartic interaction defines an ordered phase, but below four dimensions that interaction is relevant and generally leads to the [Wilson-Fisher fixed point](../../../../../wilson-fisher-fixed-point.md), not these Gaussian thermodynamic powers.

For the [Gaussian specific-heat infrared threshold](../../../../../gaussian-specific-heat-infrared-threshold.md), at $D=4$ the same [determinant](../../../../../determinant.md) integral grows like $\log(\Lambda^2/t)$, so $\alpha=0$ as a power exponent, with a logarithmic divergence. For $D>4$, it has a finite cutoff-dependent limit; the leading [heat capacity](../../../../../heat-capacity.md) is a regular constant and has no divergent power, again described by $\alpha=0$ in the requested convention. After subtraction of this background the Gaussian singular term can still have the negative power index $2-D/2$; it is not correct to erase that distinction. In a stable quartic [Landau-Ginzburg theory](../../../../../landau-ginzburg-theory.md) above four dimensions, the quartic coefficient is a [dangerously irrelevant coupling](../../../../../dangerously-irrelevant-coupling.md): it is needed for the ordered phase and contributes $f_s\propto-t^2/u$, giving the mean-field specific-heat jump and $\alpha=0$ while invalidating naive [hyperscaling relation](../../../../../hyperscaling-relation.md). At four dimensions, marginal interactions can add further logarithmic corrections. **The agreement with [Landau theory](../../../../../landau-theory.md) is in the leading heat-capacity power; it does not assert the absence of logarithms or supply a missing stable Gaussian ordered phase.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
