<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use units $\hbar=c=1$ and the [Minkowski metric](../../../../../minkowski-metric.md) $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$, so $p\cdot x=E_pt-\mathbf p\cdot\mathbf x$. The [canonical momentum](../../../../../canonical-momentum.md) of the [real scalar field](../../../../../real-scalar-field.md) is $\pi=\dot\phi$, and the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) is

$$
H=\frac12\int d^3x\,[\pi^2+(\nabla\phi)^2+m^2\phi^2].
$$

[Canonical quantization of a real scalar field](../../../../../canonical-quantization-of-a-real-scalar-field.md) promotes $\phi$ and $\pi$ to [operator-valued distributions](../../../../../operator-valued-distribution.md) satisfying the equal-time [canonical commutation relation](../../../../../canonical-commutation-relation.md)

$$
[\phi(t,\mathbf x),\pi(t,\mathbf y)]=i\delta^3(\mathbf x-\mathbf y),\qquad
[\phi(t,\mathbf x),\phi(t,\mathbf y)]=[\pi(t,\mathbf x),\pi(t,\mathbf y)]=0.
$$

Products and [operator commutators](../../../../../operator-commutator.md) can first be interpreted after spatial smearing. An additive vacuum constant in $H$ does not affect the following equations. In the [Heisenberg picture](../../../../../heisenberg-picture.md), $\dot O=i[H,O]$. Applying the [canonical commutation relation](../../../../../canonical-commutation-relation.md) to the quadratic [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), and integrating the gradient term by parts, gives

$$
\dot\phi=\pi,\qquad \dot\pi=\nabla^2\phi-m^2\phi,qquad
\boxed{(\Box+m^2)\phi=0}.
$$

Thus the [Klein-Gordon equation](../../../../../klein-gordon-equation.md) is an operator equation. The spatial [Fourier transform](../../../../../fourier-transform.md) reduces it to $\ddot\phi_{\mathbf p}+E_p^2\phi_{\mathbf p}=0$, with $E_p=\sqrt{\mathbf p^2+m^2}$. Its two frequency branches, together with the [Hermitian adjoint](../../../../../adjoint-operator.md) condition $\phi^\dagger=\phi$, give the [mode expansion of a free field](../../../../../mode-expansion-of-a-free-field.md)

$$
\phi(x)=\int d\mu(p)\,[a(\mathbf p)f_p(x)+a^\dagger(\mathbf p)f_p^*(x)],\qquad
d\mu(p)=\frac{d^3p}{(2\pi)^3 2E_p},\qquad f_p=e^{-ip\cdot x}.
$$

The measure $d\mu(p)$ is [Lorentz invariant](../../../../../lorentz-invariance.md); its normalization fixes that of the [creation and annihilation operators](../../../../../creation-and-annihilation-operators.md) rather than imposing any extra physical assumption.

For [invariant-normalized scalar mode extraction](../../../../../invariant-normalized-scalar-mode-extraction.md), take the [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md) of $f_p$ with the field. The positive-frequency contribution has coefficient $E_p+E_q$ and spatial integral $(2\pi)^3\delta^3(\mathbf p-\mathbf q)$. The negative-frequency contribution has coefficient $E_p-E_q$ and spatial integral $(2\pi)^3\delta^3(\mathbf p+\mathbf q)$, so it vanishes because $E_{-p}=E_p$. Consequently

$$
i\int d^3x\,[f_p^*\dot\phi-\phi\dot f_p^*]
=\int d\mu(q)\,(E_p+E_q)(2\pi)^3\delta^3(\mathbf p-\mathbf q)a(\mathbf q)
=a(\mathbf p).
$$

Taking the [Hermitian adjoint](../../../../../adjoint-operator.md), with the order of the scalar factors immaterial, yields

$$
\boxed{a^\dagger(\mathbf p)=-i\int d^3x\,[f_p\dot\phi-\phi\dot f_p]}.
$$

Equivalently $a(\mathbf p)=\int d^3x\,f_p^*(E_p\phi+i\pi)$ and $a^\dagger(\mathbf q)=\int d^3y\,f_q(E_q\phi-i\pi)$. At a common time their [operator commutator](../../../../../operator-commutator.md) therefore is

$$
[a(\mathbf p),a^\dagger(\mathbf q)]
=\int d^3x\,d^3y\,f_p^*(t,\mathbf x)f_q(t,\mathbf y)(E_p+E_q)\delta^3(\mathbf x-\mathbf y)
=\boxed{(2\pi)^3 2E_p\delta^3(\mathbf p-\mathbf q)}.
$$

The same calculation gives $[a(\mathbf p),a(\mathbf q)]=[a^\dagger(\mathbf p),a^\dagger(\mathbf q)]=0$: the surviving factor is an energy difference supported at opposite spatial momenta. These are the bosonic [canonical commutation relations](../../../../../canonical-commutation-relation.md) in [relativistic normalization of a one-particle state](../../../../../relativistic-normalization-of-a-one-particle-state.md).

Choose the [Fock vacuum](../../../../../fock-vacuum.md) by $a(\mathbf p)|0\rangle=0$ and $\langle0|0\rangle=1$. Only the annihilator-creator product contributes to the [Wightman function](../../../../../wightman-function.md), giving

$$
\langle0|\phi(x)\phi(y)|0\rangle=\int d\mu(p)\,e^{-ip\cdot(x-y)}.
$$

Using [time ordering](../../../../../time-ordering.md) and the reverse product for $y^0>x^0$, the [Feynman propagator](../../../../../feynman-propagator.md), with the convention $D_F=i\Delta_F$ in this calculation, is

$$
\boxed{D_F(x-y)=\int d\mu(p)\,[\theta(x^0-y^0)e^{-ip\cdot(x-y)}+\theta(y^0-x^0)e^{-ip\cdot(y-x)}]}.
$$

In particular the denominator in the spatial measure is $2E_p$ in both terms.

To verify the four-dimensional [Fourier transform](../../../../../fourier-transform.md) representation, let $\tau=x^0-y^0$ and integrate the energy variable first:

$$
I(\tau)=\lim_{\epsilon\downarrow0}\int_{-\infty}^{\infty}\frac{dp^0}{2\pi}\,
\frac{i e^{-ip^0\tau}}{(p^0)^2-E_p^2+i\epsilon}.
$$

The [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md) puts the positive-energy pole at $E_p-i0$ and the negative-energy pole at $-E_p+i0$. For $\tau>0$, the [contour integral](../../../../../contour-integral.md) closes in the lower half-plane with clockwise orientation. The [residue theorem](../../../../../residue-theorem.md) multiplies the residue $i e^{-iE_p\tau}/(2E_p)$ by $-i$, giving $e^{-iE_p\tau}/(2E_p)$. For $\tau<0$, it closes counterclockwise above: multiplying the residue $-i e^{iE_p\tau}/(2E_p)$ by $i$ gives $e^{iE_p\tau}/(2E_p)$. Thus $I(\tau)=e^{-iE_p|\tau|}/(2E_p)$. After inserting the spatial exponential, reversing $\mathbf p$ in the negative-time term gives exactly the [time ordering](../../../../../time-ordering.md) expression above. Hence

$$
\boxed{i\Delta_F(x-y)=\lim_{\epsilon\downarrow0}\int\frac{d^4p}{(2\pi)^4}\,\frac{i e^{-ip\cdot(x-y)}}{p^2-m^2+i\epsilon}}.
$$

This equality is understood as a [distribution](../../../../../distribution-mathematical-analysis.md) limit; the same prescription gives $(\Box+m^2)D_F(x-y)=-i\delta^4(x-y)$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
