<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Canonical mode mixing and its inverse.** Treat annihilation operators as column vectors and keep complex conjugation, transpose and Hermitian adjoint distinct. Computing the [canonical commutation relations](../../../../../canonical-commutation-relation.md) for $a'=\alpha a+\beta a^\dagger$ gives

$$
[a'_i,a_j'{}^\dagger]
=\sum_k(\alpha_{ik}\overline{\alpha_{jk}}-\beta_{ik}\overline{\beta_{jk}}),
\qquad
[a'_i,a'_j]=\sum_k(\alpha_{ik}\beta_{jk}-\beta_{ik}\alpha_{jk}).
$$

Consequently the required conditions are

$$
\boxed{\alpha\alpha^\dagger-\beta\beta^\dagger=I,\qquad
\alpha\beta^T=\beta\alpha^T.}
$$

For complete invertible mode mixing, put

$$
\mathcal T=
\begin{pmatrix}\alpha&\beta\\\overline\beta&\overline\alpha\end{pmatrix},
\qquad J=\begin{pmatrix}I&0\\0&-I\end{pmatrix}.
$$

The [canonical identities for a bosonic Bogoliubov transformation](../../../../../canonical-identities-for-a-bosonic-bogoliubov-transformation.md) are $\mathcal T J\mathcal T^\dagger=J$, giving $\mathcal T^{-1}=J\mathcal T^\dagger J$. Its upper blocks yield

$$
\boxed{A=\alpha^\dagger,\qquad B=-\beta^T,\qquad
A_{ij}=\overline{\alpha_{ji}},\quad B_{ij}=-\beta_{ji}.}
$$

Equivalently, the column identities are $\alpha^\dagger\alpha-\beta^T\overline\beta=I$ and $\alpha^\dagger\beta=\beta^T\overline\alpha$. In finite dimension invertibility follows from the canonical matrix identity. In infinitely many modes, the row identities alone need not give a complete inverse: $a'_i=a_{i+1}$ preserves them but discards one mode. Here completeness of the two field-mode expansions supplies the needed invertible transformation.

**Obtaining coefficients from the modes.** Use the [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md), antilinear in its first argument,

$$
(f,g)_{\rm KG}
=i\int_\Sigma d\Sigma^\mu
\left(\overline f\,\nabla_\mu g-g\nabla_\mu\overline f\right).
$$

The normalized [positive-frequency solutions](../../../../../positive-frequency-solution.md) satisfy $(p_i,p_j)=\delta_{ij}$, $(\overline p_i,\overline p_j)=-\delta_{ij}$ and $(p_i,\overline p_j)=0$. Current conservation makes this product independent of the [Cauchy hypersurface](../../../../../cauchy-surface.md) when boundary flux vanishes. Taking the product of the field with a mode gives $a_i=(p_i,\widehat\Phi)$ and hence

$$
\boxed{\alpha_{ij}=(p'_i,p_j)_{\rm KG},\qquad
\beta_{ij}=(p'_i,\overline p_j)_{\rm KG}.}
$$

With this operator convention, the corresponding mode expansion is

$$
\boxed{p'_i=\sum_j\left(\overline{\alpha_{ij}}p_j-
\overline{\beta_{ij}}\,\overline p_j\right).}
$$

The minus sign comes from the negative norm of conjugate modes. Using a different convention for mode coefficients can move this sign and the complex conjugates; the operator formula fixes them unambiguously here.

**Particle count.** In the [in-vacuum](../../../../../in-vacuum.md), only the contraction $\langle0|a_j a_k^\dagger|0\rangle=\delta_{jk}$ survives. Therefore

$$
\boxed{\langle0|a_i'{}^\dagger a'_i|0\rangle=\sum_j|\beta_{ij}|^2.}
$$

This is [particle number from Bogoliubov coefficients](../../../../../particle-number-from-bogoliubov-coefficients.md): the old vacuum contains that expected number of particles in the new mode $i$. Nonzero negative-frequency mixing is the source of particle production. For continuum modes one uses normalized wave packets and replaces the sum by the corresponding integral.

**The squeezed-state relation.** First use finitely many modes, or an implementable infinite-mode limit. Seek

$$
|\psi\rangle=C e^{\widehat F}|0'\rangle,\qquad
\widehat F=\frac12\sum_{ij}M_{ij}a_i'{}^\dagger a_j'{}^\dagger,
\qquad M=M^T.
$$

The [canonical commutation relations](../../../../../canonical-commutation-relation.md) give

$$
[a'_i,\widehat F]=\sum_jM_{ij}a_j'{}^\dagger.
$$

All further nested commutators vanish since $\widehat F$ contains only [creation operators](../../../../../creation-operator.md). Thus

$$
a_i e^{\widehat F}|0'\rangle
=e^{\widehat F}\sum_j(AM+B)_{ij}a_j'{}^\dagger|0'\rangle.
$$

The old annihilation conditions hold exactly when

$$
\boxed{M=-A^{-1}B=(\alpha^\dagger)^{-1}\beta^T.}
$$

The inverse transformation's canonical identity $AB^T=BA^T$ shows $A^{-1}B=(A^{-1}B)^T$, so the required symmetry is automatic. Also $AA^\dagger-BB^\dagger=I$ gives

$$
I-MM^\dagger=A^{-1}(A^{-1})^\dagger>0.
$$

Hence the singular values of $M$ are less than one. The [Autonne-Takagi factorization](../../../../../autonne-takagi-factorization.md) $M=U\operatorname{diag}(s_j)U^T$ changes to independent canonical oscillators. For each factor, the squared norm of $\exp(s_j b_j^{\dagger2}/2)|0\rangle$ is the even-occupation series

$$
\sum_{n=0}^\infty\frac{(2n)!}{2^{2n}(n!)^2}s_j^{2n}=(1-s_j^2)^{-1/2}.
$$

Multiplying these norms gives the finite-mode normalization

$$
\boxed{|C|=\det(I-MM^\dagger)^{1/4}.}
$$

The phase of $C$ is arbitrary. The resulting [multimode squeezed vacuum](../../../../../multimode-squeezed-vacuum.md) is annihilated by all old annihilation operators, so uniqueness of the normalized [Fock vacuum](../../../../../fock-vacuum.md) identifies it with $|0\rangle$.

The PDF's squeezed-vacuum claim needs qualification for infinitely many modes. [Bosonic mode mixing implementability](../../../../../bosonic-mode-mixing-implementability.md) requires $\beta$ to be a [Hilbert-Schmidt operator](../../../../../hilbert-schmidt-operator.md), $\sum_{ij}|\beta_{ij}|^2<\infty$, for a common ordinary [bosonic Fock space](../../../../../bosonic-fock-space.md). For a counterexample, take $\alpha=\cosh s\,I$ and $\beta=\sinh s\,I$ on countably many modes with fixed $s>0$. The algebraic canonical conditions hold, but $M=\tanh s\,I$ and the finite-$N$ normalization is $C_N=(\cosh s)^{-N/2}\to0$. Every mode has a fixed positive probability of nonzero occupation in the required product state; the probability that all but finitely many modes are empty is zero. Ordinary [Fock space](../../../../../fock-space.md) vectors instead have total occupation finite with probability one, even if their expected occupation is infinite. Thus there is no nonzero common-Fock-space vector of the prescribed form. **The squeezed expression is a normalizable vacuum relation with a finite-mode regulator or the implementability condition, not solely from the commutator identities.**

**Black-hole radiation.** In a collapse spacetime, choose early [positive-frequency solutions](../../../../../positive-frequency-solution.md) with respect to affine incoming time $v$ on [past null infinity](../../../../../past-null-infinity.md), and late outgoing modes proportional to $e^{-i\omega u}$ on [future null infinity](../../../../../future-null-infinity.md). The early state is their [in-vacuum](../../../../../in-vacuum.md). The [Hawking exponential ray map](../../../../../hawking-exponential-ray-map.md) has

$$
v_H-v=C_0e^{-\kappa u}
$$

for late outgoing rays, with $\kappa>0$. Tracing a late mode backwards therefore gives a profile proportional to

$$
\mathbf1_{\{v<v_H\}}(v_H-v)^{i\omega/\kappa}.
$$

It is not a pure positive-frequency incoming wave, so the [Bogoliubov transformation](../../../../../bogoliubov-transformation.md) has nonzero $\beta$.

To see the thermal factor, put $x=v_H-v>0$ and $a=\omega/\kappa$. The positive- and negative-frequency Fourier pieces have, apart from common normalization and phases, the regulated integrals

$$
I_\pm=\int_0^\infty x^{ia}e^{-(\varepsilon\pm i\omega')x}\,dx
=\Gamma(1+ia)(\varepsilon\pm i\omega')^{-1-ia},
\qquad \varepsilon>0.
$$

As $\varepsilon\downarrow0$, the positive-frequency piece has squared-modulus factor $e^{+\pi a}$ and the negative-frequency piece has $e^{-\pi a}$. Consequently the [thermal ratio of Hawking Bogoliubov coefficients](../../../../../thermal-ratio-of-hawking-bogoliubov-coefficients.md) is

$$
\boxed{|\beta_{\omega\omega'}|^2
=e^{-2\pi\omega/\kappa}|\alpha_{\omega\omega'}|^2.}
$$

For a normalized narrow-frequency outgoing wave packet, combine this ratio with $\sum_j(|\alpha_{ij}|^2-|\beta_{ij}|^2)=1$. The occupation is the [Bose-Einstein distribution](../../../../../bose-einstein-distribution.md)

$$
\boxed{\langle N_\omega\rangle
=\frac1{e^{2\pi\omega/\kappa}-1},\qquad
T_H=\frac{\kappa}{2\pi}.}
$$

The [Hawking temperature](../../../../../hawking-temperature.md) is thus the same one found by Euclidean regularity. For Schwarzschild, $\kappa=1/(4M)$ gives $T_H=1/(8\pi M)$ in natural units. Propagation through the exterior potential multiplies the asymptotic occupation by the [greybody factor](../../../../../greybody-factor.md) $\Gamma_\ell(\omega)$.

The outgoing radiation has partner-mode correlations across the horizon: the total state can be pure while the reduced outgoing state is thermal. A complete mode basis must include modes entering the horizon as well as those reaching infinity. The particle statement is made for normalized packets and finite observation intervals; idealized infinite-duration emission need not define the two vacua in one global [Fock space](../../../../../fock-space.md). This explains both the squeezed-state structure and the physically measurable [Hawking radiation](../../../../../hawking-radiation.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
