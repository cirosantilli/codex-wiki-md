<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

On the polynomial subspace of $L^2(\gamma)$, the [Gaussian creation and annihilation operators](../../../../../gaussian-creation-and-annihilation-operators.md) are $a^-=D$ and $a^+=x-D$. [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md) makes them adjoints there and gives $[a^-,a^+]=I$. The [Gaussian number operator](../../../../../gaussian-number-operator.md) is

$$
\boxed{N=a^+a^-=-D^2+xD.}
$$

The [Probabilists' Hermite polynomials](../../../../../probabilists-hermite-polynomial.md) are $\operatorname{He}_n(x)=(-1)^ne^{x^2/2}D^ne^{-x^2/2}=(a^+)^n1$. Their generating function is $e^{sx-s^2/2}=\sum_n\operatorname{He}_n(x)s^n/n!$, giving $D\operatorname{He}_n=n\operatorname{He}_{n-1}$. The commutator also yields

$$
\boxed{N\operatorname{He}_n=n\operatorname{He}_n,\qquad\int\operatorname{He}_m\operatorname{He}_n\,d\gamma=n!\,\mathbf1_{m=n}.}
$$

The orthogonality follows by repeated [integration by parts](../../../../../integration-by-parts.md); the leading coefficient is one, so these polynomials span every polynomial. By the allowed density assumption $h_n=\operatorname{He}_n/\sqrt{n!}$ is an [orthonormal basis](../../../../../orthonormal-basis.md). Define the closed number operator by $N\sum c_nh_n=\sum nc_nh_n$ on $\sum n^2|c_n|^2<\infty$. This diagonal [multiplication operator](../../../../../multiplication-operator.md) is self-adjoint and positive semidefinite; polynomial truncations show it is the closure of the polynomial operator.

The [Ornstein-Uhlenbeck semigroup](../../../../../ornstein-uhlenbeck-semigroup.md) is $P_t=e^{-tN}$, or $P_tf=\sum_ne^{-nt}c_nh_n$. It also has the [Mehler formula for the Ornstein-Uhlenbeck semigroup](../../../../../mehler-formula-for-the-ornstein-uhlenbeck-semigroup.md)

$$
\boxed{P_tf(x)=\mathbb E\left[f\!\left(e^{-t}x+\sqrt{1-e^{-2t}}\,Z\right)\right],\qquad Z\sim N(0,1).}
$$

To verify the formula, apply its right side to $e^{sx-s^2/2}$: the [Gaussian moment-generating function](../../../../../moment-generating-function-of-a-normal-distribution.md) makes the result $e^{se^{-t}x-s^2e^{-2t}/2}$, proving the [eigenvalue](../../../../../eigenvalue.md) identity on every Hermite polynomial. [Positivity](../../../../../positivity-linear-maps.md) and invariance of [Gaussian measure](../../../../../gaussian-measure.md) give $L^2$ contraction by [Jensen inequality](../../../../../jensen-s-inequality.md), so polynomial density extends the equality to all $L^2(\gamma)$. The coefficient expansion gives

$$
\|P_tf-\mathbb E_\gamma f\|_2^2=\sum_{n\geq1}e^{-2nt}|c_n|^2\longrightarrow0.
$$

For continuously differentiable $f$ with bounded [derivative](../../../../../derivative.md), differentiate the Mehler expectation by the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) to get the [Ornstein-Uhlenbeck gradient commutation identity](../../../../../ornstein-uhlenbeck-gradient-commutation-identity.md)

$$
\boxed{(P_tf)'=e^{-t}P_t(f').}
$$

The same identity extends to the [Gaussian Sobolev form domain](../../../../../gaussian-sobolev-space.md). Mehler's formula also gives [pointwise convergence](../../../../../pointwise-convergence.md) to the Gaussian mean for such $f$, since bounded [derivative](../../../../../derivative.md) permits at most linear growth.

The [Gaussian Dirichlet energy](../../../../../gaussian-dirichlet-energy.md) is the energy form of $N$:

$$
\boxed{\mathcal E_\gamma(f)=\lim_{t\downarrow0}\frac{\|f\|_2^2-\langle f,P_tf\rangle}{t}=\sum_{n\geq1}n|c_n|^2=\int|f'|^2\,d\gamma.}
$$

For polynomials this follows from $N=(a^-)^*a^-$, and closure extends it to the form domain. For the given continuously differentiable $f$, [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md) yields $\langle f',h_{n-1}\rangle=\sqrt n c_n$, so [Parseval identity](../../../../../parseval-identity.md) proves the derivative-energy equality directly. Bounded [derivative](../../../../../derivative.md) puts $f$ in the [Gaussian Sobolev space](../../../../../gaussian-sobolev-space.md), hence in that form domain; it need not be in the full [operator domain](../../../../../operator-domain.md), so $\langle f,Nf\rangle$ is not always a legitimate initial definition.

Use the [entropy functional](../../../../../entropy-functional.md) $\operatorname{Ent}_\gamma(h)=\int h\log h\,d\gamma-(\int h\,d\gamma)\log\int h\,d\gamma$. Begin with bounded smooth $h>0$ bounded away from zero, and put $h_t=P_th$. Invariance and [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md) give the [Ornstein-Uhlenbeck entropy dissipation identity](../../../../../ornstein-uhlenbeck-entropy-dissipation-identity.md)

$$
-\frac{d}{dt}\operatorname{Ent}_\gamma(h_t)=\int\frac{|h_t'|^2}{h_t}\,d\gamma.
$$

The gradient identity and the permitted weighted [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), applied with weight $h$, imply

$$
\frac{|h_t'|^2}{h_t}=e^{-2t}\frac{|P_t(h')|^2}{P_th}\leq e^{-2t}P_t\!\left(\frac{|h'|^2}{h}\right).
$$

The entropy tends to zero as $t\to\infty$ by Mehler's formula and bounded convergence. Integrating in time and using invariance yields $\operatorname{Ent}_\gamma(h)\leq\frac12\int|h'|^2/h\,d\gamma$. Set $h=f^2$ to obtain the sharp [Gaussian logarithmic Sobolev inequality](../../../../../gaussian-logarithmic-sobolev-inequality.md)

$$
\boxed{\operatorname{Ent}_\gamma(f^2)\leq2\int|f'|^2\,d\gamma=2\mathcal E_\gamma(f).}
$$

For the stated possibly unbounded $f$, apply the argument to smooth positive clipped approximations with a common positive lower bound and uniformly bounded [derivatives](../../../../../derivative.md). They can converge pointwise together with their [derivatives](../../../../../derivative.md) and have a common linear-growth bound. Since [Gaussian measure](../../../../../gaussian-measure.md) integrates every polynomial moment, [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) passes both the entropy and the [derivative](../../../../../derivative.md) energy to the limit. This also justifies use of the supplied inequality when $2ff'$ itself is unbounded. The normalization $\|f\|_1=1$ concerns $f$, and does not imply $\int f^2\,d\gamma=1$; the second term in the entropy definition must be retained.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
