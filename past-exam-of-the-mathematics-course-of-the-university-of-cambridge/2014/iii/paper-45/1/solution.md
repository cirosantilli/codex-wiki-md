<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the metric $g^{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$ and the usual [Dirac basis](../../../../../dirac-representation-of-the-gamma-matrices.md), with $(\gamma^0)^\dagger=\gamma^0$ and $(\gamma^i)^\dagger=-\gamma^i$. In this solution the sign of the [chirality matrix](../../../../../chirality-matrix.md) is the one specified in the paper, $\gamma^5=-i\gamma^0\gamma^1\gamma^2\gamma^3$. Define $t_0=1$ and $t_i=-1$, with no summation in componentwise transformation formulas.

Complex conjugation changes the explicit $-i$ to $+i$. Three spatial [gamma matrices](../../../../../gamma-matrices.md) each contribute another minus sign, so

$$
B\gamma^{5*}B^{-1}=i\gamma^0(-\gamma^1)(-\gamma^2)(-\gamma^3)=-i\gamma^0\gamma^1\gamma^2\gamma^3=\boxed{\gamma^5}.
$$

Also $(\gamma^5)^2=1$ and $\{\gamma^5,\gamma^\mu\}=0$ by the [Clifford algebra](../../../../../clifford-algebra.md).

The [quantum time-reversal operator](../../../../../quantum-time-reversal-operator.md) is [antiunitary](../../../../../antiunitary-operator.md): it conjugates numerical coefficients, including the [Dirac spinors](../../../../../dirac-spinor.md) and plane-wave exponentials in the [mode expansion of a Dirac field](../../../../../mode-expansion-of-a-dirac-field.md). To fix the spin phase explicitly, put $\epsilon_s=(-1)^{1/2-s}$ and use

$$
\hat T b^s(p)\hat T^{-1}=\epsilon_s b^{-s}(p_T),\qquad
\hat T d^{s\dagger}(p)\hat T^{-1}=\epsilon_s d^{-s\dagger}(p_T).
$$

This convention gives $\hat T^2=-1$ on a one-fermion state, since $\epsilon_s\epsilon_{-s}=-1$. In the transformed expansion, change variables from $(p,s)$ to $(p_T,-s)$. The [Lorentz-invariant phase-space measure](../../../../../lorentz-invariant-phase-space-measure.md) is unchanged, and $p_T\cdot x=-p\cdot x_T$. The coefficient of $b^s(p)e^{-ip\cdot x_T}$ is therefore

$$
\epsilon_{-s}u^{-s*}(p_T)=-\epsilon_su^{-s*}(p_T)=\gamma^5Cu^s(p).
$$

The same calculation applies to the antiparticle coefficient. Thus, with this explicitly fixed spin convention,

$$
\boxed{B=\gamma^5C,\qquad \hat T\psi(x)\hat T^{-1}=B\psi(x_T).}
$$

The [spin phase in the Dirac time-reversal matrix](../../../../../spin-phase-in-the-dirac-time-reversal-matrix.md) matters here: a common change of the one-particle time-reversal phase replaces $B$ by $-B$; the phase-independent relation is $B\propto\gamma^5C$. It changes neither the defining conjugation property nor any bilinear result below. Normalize $B$ to be a [unitary matrix](../../../../../unitary-matrix.md). In the [Dirac basis](../../../../../dirac-representation-of-the-gamma-matrices.md), $\gamma^0$ is real and commutes with $B$, so transforming the [Dirac adjoint](../../../../../dirac-adjoint.md) gives

$$
\hat T\bar\psi(x)\hat T^{-1}=(B\psi(x_T))^\dagger\gamma^{0*}
=\psi^\dagger(x_T)B^{-1}\gamma^0
=\boxed{\bar\psi(x_T)B^{-1}}.
$$

Here complex conjugation of the matrix defining the [Dirac adjoint](../../../../../dirac-adjoint.md) is essential. An explicit realization consistent with the sign of $\gamma^5$ used here is $C=i\gamma^2\gamma^0$ and $B=\gamma^1\gamma^3$; it has $B^{-1}=-B$, so conjugation by $B$ and by $B^{-1}$ coincides. The usual changes of [Dirac spinor](../../../../../dirac-spinor.md) basis by [unitary matrices](../../../../../unitary-matrix.md) carry the adjoint and time-reversal matrix with them.

For the [charge-conjugation matrix](../../../../../charge-conjugation-matrix.md), the [gamma matrix adjoint and transpose identities](../../../../../gamma-matrix-adjoint-and-transpose-identities.md) give $\gamma^{\mu T}=t_\mu\gamma^{\mu*}$. Consequently $B\gamma^{\mu T}B^{-1}=\gamma^\mu$. Since $C=\gamma^5B$ in the chosen phase convention,

$$
C\gamma^{\mu T}C^{-1}=\gamma^5B\gamma^{\mu T}B^{-1}\gamma^5
=\gamma^5\gamma^\mu\gamma^5=\boxed{-\gamma^\mu}.
$$

This proof uses a temporal [Hermitian matrix](../../../../../hermitian-operator.md) and spatial [skew-Hermitian matrices](../../../../../skew-hermitian-matrix.md) explicitly; the transpose identity is preserved when $C$ is transformed appropriately with the [gamma matrices](../../../../../gamma-matrices.md).

For the [Fermi interaction](../../../../../fermi-interaction.md), let $V_{pn}^\mu=\bar p\gamma^\mu n$ and $A_{pn}^\mu=\bar p\gamma^\mu\gamma^5 n$. In the displayed [Dirac basis](../../../../../dirac-representation-of-the-gamma-matrices.md), the inverse version of the conjugation relation also holds. [Antiunitarity](../../../../../antiunitary-operator.md), $B^{-1}\gamma^{\mu*}B=t_\mu\gamma^\mu$ and $B^{-1}\gamma^{5*}B=\gamma^5$ give

$$
\hat T V_{pn}^\mu(x)\hat T^{-1}=t_\mu V_{pn}^\mu(x_T),\qquad
\hat T A_{pn}^\mu(x)\hat T^{-1}=t_\mu A_{pn}^\mu(x_T).
$$

The leptonic [weak charged current](../../../../../charged-current.md) has the same component signs. In the contraction of leptonic and hadronic currents, the two $t_\mu$ factors cancel. Its two independent operators thus keep their form while their coefficients become $g_V^*$ and $g_A^*$. The Hermitian-conjugate term transforms separately; its presence does not remove a relative complex phase between the vector and axial couplings.

With all intrinsic phases fixed to one and a real positive [Fermi constant](../../../../../fermi-constant.md), invariance requires real coefficients in that convention. A common phase of $g_V$ and $g_A$ can instead be absorbed into a rephasing of the nucleon fields, and hence into their intrinsic time-reversal phases. The convention-independent condition, for $g_V\ne0$, is

$$
\boxed{\operatorname{Im}(g_Ag_V^*)=0,\qquad g_A/g_V\in\mathbb R.}
$$

This is the [relative weak phase condition for time reversal](../../../../../relative-weak-phase-condition-for-time-reversal.md). If one coefficient vanishes, there is no relative phase to constrain; the remaining common phase can be removed. A nonreal ratio violates [time-reversal symmetry](../../../../../t-symmetry.md) even though the [Lagrangian density](../../../../../lagrangian-density.md) includes its Hermitian conjugate.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 45](../../paper-45-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
