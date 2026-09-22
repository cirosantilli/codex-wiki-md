<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use signature $(+---)$ and covariant [one-particle state](../../../../../one-particle-state.md) normalization $\langle p'|p\rangle=(2\pi)^3 2E_p\delta^3(\mathbf p-\mathbf p')$. The future scattering condition uses the outgoing [asymptotic scalar field](../../../../../asymptotic-scalar-field.md):

$$
\boxed{\phi(x)\longrightarrow\sqrt Z\,\phi_{\rm out}(x)\quad(x^0\to+\infty),\qquad
(\partial^2+m^2)\phi_{\rm out}=0.}
$$

As with the incoming condition, this is understood in suitably smeared scattering matrix elements, not as unrestricted pointwise strong convergence of interacting and free local operators.

The free incoming field has expansion

$$
\phi_{\rm in}(x)=\int\frac{d^3\mathbf k}{(2\pi)^3 2E_k}
\left[a_{\rm in}(k)e^{-ikx}+a_{\rm in}^\dagger(k)e^{ikx}\right],\qquad
[a_{\rm in}(k),a_{\rm in}^\dagger(p)]=(2\pi)^3 2E_k\delta^3(\mathbf k-\mathbf p).
$$

The [creation operator](../../../../../creation-operator.md) defines $|p\rangle=a_{\rm in}^\dagger(p)|0\rangle$, with $a_{\rm in}|0\rangle=0$, so $\langle p|\phi_{\rm in}(x)|0\rangle=e^{ipx}$. On the other hand, [translation invariance](../../../../../translation-invariance.md) gives

$$
\phi(x)=e^{iPx}\phi(0)e^{-iPx},\qquad
\langle p|\phi(x)|0\rangle=e^{ipx}\langle p|\phi(0)|0\rangle.
$$

Matching the stable [one-particle state](../../../../../one-particle-state.md) component in the asymptotic condition fixes the constant overlap. Choose its state phase so that it is real and nonnegative. Then

$$
\boxed{\langle p|\phi(0)|0\rangle=\sqrt Z.}
$$

The same stable particle appears in the outgoing description, with compatible one-particle phases. Thus $Z$ is the squared overlap measured by [wave-function renormalization](../../../../../wave-function-renormalization.md).

Insert a complete set of [four-momentum](../../../../../four-momentum.md) eigenstates between the fields. For $x^0>0$, [translation invariance](../../../../../translation-invariance.md) and Hermiticity give

$$
\langle0|\phi(x)\phi(0)|0\rangle
=\sum_\alpha e^{-ip_\alpha x}|\langle\alpha|\phi(0)|0\rangle|^2.
$$

For $x^0<0$, reversing the [time-ordered product](../../../../../time-ordered-product.md) gives the same sum with $e^{ip_\alpha x}$. Therefore, with continuous-state integrals implicit in the completeness sum,

$$
i\Delta(x)=\sum_\alpha |\langle\alpha|\phi(0)|0\rangle|^2
\left[\theta(x^0)e^{-ip_\alpha x}+\theta(-x^0)e^{ip_\alpha x}\right].
$$

Here $\theta$ is the [Heaviside step function](../../../../../heaviside-step-function.md).

For the usual spectral representation, take a Lorentz-invariant vacuum, a positive-norm [Hilbert space](../../../../../hilbert-space-split.md) and the future-cone [spectrum condition](../../../../../spectrum-condition.md). Also take $\langle0|\phi|0\rangle=0$, as for the unbroken real scalar field, or subtract this constant and use the [connected correlation function](../../../../../connected-correlation-function.md). Otherwise the vacuum intermediate state adds a disconnected constant not represented by the ordinary mass-shell measure below.

Let $W(x)=\langle0|\phi(x)\phi(0)|0\rangle$ for that centered field, and use the [Fourier transform](../../../../../fourier-transform.md) convention $W(x)=\int d^4p\,(2\pi)^{-4}e^{-ipx}\widetilde W(p)$. Define the [Källén–Lehmann spectral density](../../../../../kallen-lehmann-spectral-density.md) by the distributional equality

$$
\widetilde W(p)=(2\pi)^4\sum_\alpha |\langle\alpha|\phi(0)|0\rangle|^2\delta^4(p-p_\alpha)
=2\pi\theta(p^0)\rho(p^2).
$$

Lorentz invariance makes the weight on each future mass shell a function or measure of $p^2$; the [spectrum condition](../../../../../spectrum-condition.md) gives $p^2\geq0$. Its nonnegativity follows from the displayed squared matrix elements. Thus

$$
W(x)=\int_0^\infty d\sigma\,\rho(\sigma)
\int\frac{d^3\mathbf p}{(2\pi)^3 2\sqrt{\mathbf p^2+\sigma}}e^{-ipx}.
$$

Applying [time ordering](../../../../../time-ordering.md) to this expression mass shell by mass shell proves the [Källén–Lehmann spectral representation](../../../../../kallen-lehmann-spectral-representation.md):

$$
\boxed{\Delta(x)=\int_0^\infty d\sigma\,\rho(\sigma)\Delta_F(x,\sigma),\qquad
\Delta_F(p,\sigma)=\frac1{p^2-\sigma+i0}.}
$$

The factor $i$ is outside $\Delta_F$ under the convention in the question.

The stable [one-particle state](../../../../../one-particle-state.md) part of completeness is $\int d^3\mathbf p\,[(2\pi)^3 2E_p]^{-1}|p\rangle\langle p|$. Its overlap is $\sqrt Z$, so its contribution to $W$ is $Z$ times the free mass-$m$ two-point function. Hence

$$
\boxed{\rho(\sigma)=Z\delta(\sigma-m^2)+\rho_{\rm rest}(\sigma),\qquad \rho_{\rm rest}\geq0.}
$$

Other isolated particles as well as multiparticle states can belong to $\rho_{\rm rest}$. The full [scalar propagator](../../../../../scalar-propagator.md) accordingly has isolated pole $Z/(p^2-m^2+i0)$, making $Z$ its pole residue.

Finally use [canonical field normalization](../../../../../canonical-field-normalization.md): the [canonical momentum](../../../../../canonical-momentum.md) is $\dot\phi$ and the equal-time [canonical commutation relation](../../../../../canonical-commutation-relation.md) is $[\dot\phi(t,\mathbf x),\phi(t,\mathbf y)]=-i\delta^3(\mathbf x-\mathbf y)$. The vacuum commutator $C(x)=W(x)-W(-x)$ has the same spectral decomposition. For each free mass shell,

$$
\left.\partial_{x^0}C_\sigma(x)\right|_{x^0=0}
=-\frac i2\int\frac{d^3\mathbf p}{(2\pi)^3}
\left(e^{i\mathbf p\cdot\mathbf x}+e^{-i\mathbf p\cdot\mathbf x}\right)
=-i\delta^3(\mathbf x),
$$

independently of $\sigma$. Comparing with the interacting equal-time commutator gives the [canonical scalar spectral sum rule](../../../../../canonical-scalar-spectral-sum-rule.md):

$$
\boxed{\int_0^\infty\rho(\sigma)\,d\sigma=1,\qquad 0\leq Z\leq1.}
$$

For the particle genuinely interpolated by the stated asymptotic field, $Z>0$; the general nonnegative bound allows a field with zero overlap. The total weight and the upper bound require this canonical normalization and a well-defined distributional equal-time limit. They do not follow from the asymptotic condition alone: rescaling $\phi$ rescales both $Z$ and the entire spectral measure.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
