<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $\eta_{ab}=\operatorname{diag}(1,-1,-1,-1)$ and $\hbar=1$. The free [real scalar field](../../../../../real-scalar-field.md) has [action](../../../../../action.md)

$$
S=\frac12\int d^4x\,[\partial_a\phi\partial^a\phi-m^2\phi^2].
$$

The [canonical momentum](../../../../../canonical-momentum.md) is $\pi=\partial\mathcal L/\partial\dot\phi=\dot\phi$, and the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) is obtained by the [Legendre transform](../../../../../convex-conjugate.md) of the density:

$$
H=\frac12\int d^3x\,[\pi^2+(\boldsymbol\nabla\phi)^2+m^2\phi^2].
$$

[Canonical quantization](../../../../../canonical-quantization.md) promotes $\phi$ and $\pi$ to Hermitian operator-valued fields and imposes the equal-time [canonical commutation relations](../../../../../canonical-commutation-relation.md)

$$
[\phi(t,\mathbf x),\pi(t,\mathbf y)]=i\delta^3(\mathbf x-\mathbf y),\qquad
[\phi(t,\mathbf x),\phi(t,\mathbf y)]=[\pi(t,\mathbf x),\pi(t,\mathbf y)]=0.
$$

Their [Heisenberg equation of motion](../../../../../heisenberg-equation-of-motion.md) gives $\dot\phi=\pi$, $\dot\pi=\boldsymbol\nabla^2\phi-m^2\phi$, hence the [Klein-Gordon equation](../../../../../klein-gordon-equation.md) $(\Box+m^2)\phi=0$.

Let $E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}$ and $p\cdot x=E_{\mathbf p}t-\mathbf p\cdot\mathbf x$. The Hermitian field mode expansion is

$$
\phi(x)=\int\frac{d^3p}{(2\pi)^3\sqrt{2E_{\mathbf p}}}
\left[a(\mathbf p)e^{-ip\cdot x}+a^\dagger(\mathbf p)e^{ip\cdot x}\right].
$$

The [scalar field oscillator inversion](../../../../../scalar-field-oscillator-inversion.md) extracts

$$
a(\mathbf p)=e^{iE_{\mathbf p}t}\int d^3x\,e^{-i\mathbf p\cdot\mathbf x}
\left[\sqrt{\frac{E_{\mathbf p}}2}\,\phi(t,\mathbf x)+\frac{i}{\sqrt{2E_{\mathbf p}}}\,\pi(t,\mathbf x)\right],
$$

and its adjoint obtained by [Hermitian conjugation](../../../../../hermitian-conjugation.md) extracts $a^\dagger$. Substitute these expressions into the equal-time [canonical commutation relation](../../../../../canonical-commutation-relation.md). The two mixed field-momentum terms give

$$
\begin{aligned}
[a(\mathbf p),a^\dagger(\mathbf q)]
&=e^{i(E_{\mathbf p}-E_{\mathbf q})t}\frac12
\left(\sqrt{\frac{E_{\mathbf p}}{E_{\mathbf q}}}+\sqrt{\frac{E_{\mathbf q}}{E_{\mathbf p}}}\right)
(2\pi)^3\delta^3(\mathbf p-\mathbf q)\\
&=\boxed{(2\pi)^3\delta^3(\mathbf p-\mathbf q)}.
\end{aligned}
$$

For $[a(\mathbf p),a(\mathbf q)]$, the corresponding coefficient is a difference of those square roots and multiplies $\delta^3(\mathbf p+\mathbf q)$; it vanishes because $E_{\mathbf p}=E_{-\mathbf p}$. Taking the adjoint gives $[a^\dagger,a^\dagger]=0$. Thus these are bosonic [annihilation operators](../../../../../annihilation-operator.md) and [creation operators](../../../../../creation-operator.md). The vacuum satisfies $a(\mathbf p)|0\rangle=0$, and [normal ordering](../../../../../normal-ordering.md) gives $:H:=\int d^3p\,E_{\mathbf p}a^\dagger(\mathbf p)a(\mathbf p)/(2\pi)^3$, after removing the constant zero-point energy. A one-particle excitation has [energy](../../../../../energy.md) $E_{\mathbf p}$ and spin zero.

The [Feynman propagator](../../../../../feynman-propagator.md) $G_F(x-y)=\langle0|T\phi(x)\phi(y)|0\rangle$ is the [vacuum expectation value](../../../../../vacuum-expectation-value.md) of the [time-ordered product](../../../../../time-ordered-product.md) of two field insertions. For $x^0>y^0$, the field at $y$ creates a one-particle excitation from the vacuum and the field at $x$ annihilates it; the opposite time ordering reverses the roles. It is a propagation amplitude and correlation function of vacuum fluctuations, rather than a transition probability. From the oscillator expansion, only the $a$-$a^\dagger$ contraction survives, so with $t=x^0-y^0$ and $\mathbf r=\mathbf x-\mathbf y$,

$$
\begin{aligned}
G_F(t,\mathbf r)
&=\int\frac{d^3p}{(2\pi)^3,2E_{\mathbf p}}
\left[\theta(t)e^{-iE_{\mathbf p}t+i\mathbf p\cdot\mathbf r}
+\theta(-t)e^{iE_{\mathbf p}t-i\mathbf p\cdot\mathbf r}\right]\\
&=\int\frac{d^3p}{(2\pi)^3,2E_{\mathbf p}}
 e^{i\mathbf p\cdot\mathbf r}e^{-iE_{\mathbf p}|t|}.
\end{aligned}
$$

Here $\theta$ is the [Heaviside step function](../../../../../heaviside-step-function.md), and changing $\mathbf p$ to $-\mathbf p$ in the second term gives the last line.

For the [Fourier transform](../../../../../fourier-transform.md) convention $\widetilde G_F(\omega,\mathbf p)=\int dt\,d^3r\,e^{i\omega t-i\mathbf p\cdot\mathbf r}G_F(t,\mathbf r)$, insert a positive damping factor $e^{-\epsilon|t|}$ and integrate the positive and negative half-lines separately:

$$
\widetilde G_F(\omega,\mathbf p)
=\lim_{\epsilon\downarrow0}\frac{i}{2E_{\mathbf p}}
\left[\frac1{\omega-E_{\mathbf p}+i\epsilon}-\frac1{\omega+E_{\mathbf p}-i\epsilon}\right]
=\boxed{\frac{i}{\omega^2-\mathbf p^2-m^2+i0}}.
$$

The last equality is a [distribution](../../../../../distribution-mathematical-analysis.md) identity; the infinitesimals in the partial fractions need not have the same finite magnitude as the infinitesimal in the combined denominator. The [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md) means that the positive-frequency pole is just below the real [energy](../../../../../energy.md) axis and the negative-frequency pole is just above it. Closing the [contour integral](../../../../../contour-integral.md) below for $t>0$, and above for $t<0$, reproduces the oscillator result by the [residue theorem](../../../../../residue-theorem.md). This prescription fixes which homogeneous solutions are added to the [Green function](../../../../../green-s-function.md). As an independent normalization check, $e^{-iE|t|}/(2E)$ has derivative jump $-i$ at $t=0$, so

$$
(\Box+m^2)G_F(x)=-i\delta^4(x).
$$

It is the expectation-value convention for $G_F$, including the numerator $i$, that determines this source normalization.

The vacuum is a centered free Gaussian state. The [Wick theorem](../../../../../wick-s-theorem.md) expresses the four-field [time-ordered product](../../../../../time-ordered-product.md) as the sum of all pair [Wick contractions](../../../../../wick-contraction.md) plus terms containing a [normal-ordered product](../../../../../normal-ordered-product.md). The latter terms have zero [vacuum expectation value](../../../../../vacuum-expectation-value.md). There are exactly three complete pairings, with no [fermionic signs](../../../../../fermionic-sign.md) for this bosonic field. Thus the [free scalar four-point function](../../../../../free-scalar-four-point-function.md) is

$$
\boxed{\begin{aligned}
\langle0|T\phi(x_1)\phi(x_2)\phi(x_3)\phi(x_4)|0\rangle
={}&G_F(x_1-x_2)G_F(x_3-x_4)\\
&+G_F(x_1-x_3)G_F(x_2-x_4)\\
&+G_F(x_1-x_4)G_F(x_2-x_3).
\end{aligned}}
$$

These formulas describe [canonical quantization of a real scalar field](../../../../../canonical-quantization-of-a-real-scalar-field.md); in particular, a [real scalar field](../../../../../real-scalar-field.md) uses a single oscillator family rather than independent charged-particle and antiparticle families.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
