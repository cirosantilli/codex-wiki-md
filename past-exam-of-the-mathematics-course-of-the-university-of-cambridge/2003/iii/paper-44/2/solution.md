<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [Minkowski metric](../../../../../minkowski-metric.md) $g=\operatorname{diag}(1,-1,-1,-1)$. Multiplying the block [gamma matrices](../../../../../gamma-matrices.md) and using the [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives

$$
(\gamma^0)^2=I_4,\qquad (\gamma^j)^2=-I_4,\qquad
\{\gamma^0,\gamma^j\}=0,\qquad \{\gamma^j,\gamma^l\}=-2\delta_{jl}I_4.
$$

Thus these matrices satisfy the [Clifford algebra](../../../../../clifford-algebra.md) relation $\{\gamma^\mu,\gamma^\nu\}=2g^{\mu\nu}I_4$. Since [partial derivatives](../../../../../partial-derivative.md) commute, the antisymmetric part of $\gamma^\mu\gamma^\nu$ drops out of its contraction with $\partial_\mu\partial_\nu$. Multiplying the [Dirac equation](../../../../../dirac-equation.md) on the left by $i\gamma^\mu\partial_\mu+m$ gives

$$
(i\gamma\cdot\partial+m)(i\gamma\cdot\partial-m)\psi
=-(\Box+m^2)\psi=0.
$$

Therefore **every component of the Dirac spinor obeys the Klein-Gordon equation with mass $m$**.

For [Lorentz covariance](../../../../../lorentz-covariance.md), take $x'=Lx$ and $\psi'(x')=S(L)\psi(x)$, with constant $L$ and $S$. The chain rule gives $\partial'_\mu=(L^{-1})^\nu{}_{\mu}\partial_\nu$. The given intertwining relation then implies

$$
\begin{aligned}
(i\gamma^\mu\partial'_\mu-m)\psi'(x')
&=S\left[i(S^{-1}\gamma^\mu S)(L^{-1})^\nu{}_{\mu}\partial_\nu-m\right]\psi(x)\\
&=S(i\gamma^\nu\partial_\nu-m)\psi(x)=0.
\end{aligned}
$$

This proves invariance of the [Dirac equation](../../../../../dirac-equation.md) under the joint coordinate and [spinor](../../../../../spinor.md) transformation.

The infinitesimal identity follows directly from the [spinor Lorentz generator commutator](../../../../../spinor-lorentz-generator-commutator.md). To derive it, first move $\gamma^\rho$ through a two-matrix product using the [Clifford algebra](../../../../../clifford-algebra.md):

$$
[\gamma^\mu\gamma^\nu,\gamma^\rho]
=2g^{\nu\rho}\gamma^\mu-2g^{\mu\rho}\gamma^\nu.
$$

Subtract the expression with $\mu$ and $\nu$ interchanged and multiply by $i/2$. Thus

$$
[\sigma^{\mu\nu},\gamma^\rho]
=2i(g^{\nu\rho}\gamma^\mu-g^{\mu\rho}\gamma^\nu).
$$

Writing $S=1-\frac i4\sigma^{\mu\nu}\omega_{\mu\nu}$ gives $S^{-1}=1+\frac i4\sigma^{\mu\nu}\omega_{\mu\nu}+O(\omega^2)$, and hence

$$
\begin{aligned}
S^{-1}\gamma^\rho S
&=\gamma^\rho+\frac i4\omega_{\mu\nu}[\sigma^{\mu\nu},\gamma^\rho]+O(\omega^2)\\
&=\gamma^\rho-\frac12\omega_{\mu\nu}(g^{\nu\rho}\gamma^\mu-g^{\mu\rho}\gamma^\nu)+O(\omega^2)\\
&=\gamma^\rho+\omega^\rho{}_{\nu}\gamma^\nu+O(\omega^2)
=L^\rho{}_{\nu}\gamma^\nu+O(\omega^2).
\end{aligned}
$$

The last step uses $\omega_{\mu\nu}=-\omega_{\nu\mu}$, including the metric signs in raising the first index.

For [parity symmetry in quantum field theory](../../../../../parity-symmetry-in-quantum-field-theory.md), set $y=x_P=(t,-\mathbf x)$. The time derivative of $\psi(y)$ is unchanged and each spatial derivative changes sign. Also $\gamma^0$ commutes with itself and anticommutes with every $\gamma^j$. Consequently

$$
(i\gamma^\mu\partial_\mu-m)\gamma^0\psi(x_P)
=\gamma^0(i\gamma^\mu\partial_{y^\mu}-m)\psi(y)=0.
$$

This verifies the specified [parity symmetry in quantum field theory](../../../../../parity-symmetry-in-quantum-field-theory.md) action explicitly.

For [charge conjugation](../../../../../charge-conjugation.md), put $B=i\gamma^2$, so $\psi_C=B\psi^*$. In the [Dirac representation of the gamma matrices](../../../../../dirac-representation-of-the-gamma-matrices.md), $\gamma^0,\gamma^1,\gamma^3$ are real and $\gamma^2$ is imaginary. The [Clifford algebra](../../../../../clifford-algebra.md) therefore gives $B\gamma^{\mu *}B^{-1}=-\gamma^\mu$ for all four indices. Complex conjugation of the [Dirac equation](../../../../../dirac-equation.md), followed by multiplication by $B$, yields

$$
(-i\gamma^{\mu *}\partial_\mu-m)\psi^*=0
\quad\Longrightarrow\quad
(i\gamma^\mu\partial_\mu-m)\psi_C=0.
$$

This is the [antilinear charge-conjugation intertwiner](../../../../../antilinear-charge-conjugation-intertwiner.md) property. No electromagnetic background is being held fixed in this free-field calculation.

Apply the specified [parity symmetry in quantum field theory](../../../../../parity-symmetry-in-quantum-field-theory.md) action before [charge conjugation](../../../../../charge-conjugation.md). Since $\gamma^0$ is real and $B\gamma^0=-\gamma^0B$,

$$
(\psi_P)_C(x)=B[\gamma^0\psi(x_P)]^*
=\boxed{-\gamma^0\psi_C(x_P)}.
$$

Thus the induced parity action on the charge-conjugate spinor has the opposite sign. In particular, if a spinor has [intrinsic parity](../../../../../intrinsic-parity.md) $\eta=\pm1$, its charge conjugate has intrinsic parity $-\eta$. Equivalently, at rest the positive-frequency [Dirac spinors](../../../../../dirac-spinor.md) occupy the upper two components and have $\gamma^0$ eigenvalue $+1$, whereas the negative-frequency [Dirac spinors](../../../../../dirac-spinor.md) occupy the lower two components and have eigenvalue $-1$. The corresponding particle and antiparticle creation operators inherit these opposite signs under the specified parity convention. Hence **electrons and positrons have opposite intrinsic parities**; conventionally one assigns $+1$ to the electron and $-1$ to the positron. The common real overall parity sign may be reversed without changing this relative sign, as in [opposite intrinsic parities of a Dirac particle and antiparticle](../../../../../opposite-intrinsic-parities-of-a-dirac-particle-and-antiparticle.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
