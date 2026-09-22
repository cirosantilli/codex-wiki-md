<h1 id="35b/solution">Solution</h1>

↑ **Parent:** [35B](../35b.md)

There is a sign inconsistency in the printed starting [energy](../../../../../energy.md): its kinetic term uses $\nabla+iq_sA/\hbar$, while the requested field equation, current and later zero-covariant-derivative condition use $\nabla-iq_sA/\hbar$. Both conventions can be derived explicitly. Set $D_\eta=\nabla-i\eta q_sA/\hbar$ for $\eta=\pm1$; the intended later equations take $\eta=1$, whereas the literal printed [energy](../../../../../energy.md) takes $\eta=-1$.

The magnetic term is $B^2/(2\mu_0)$, because $A_{k,j}(A_{k,j}-A_{j,k})=|\nabla\times A|^2$. Vary $\psi^*$ independently with compactly supported variations. [Integration by parts](../../../../../integration-by-parts.md) in the kinetic term gives

$$
\boxed{-\frac{\hbar^2}{2m_s}D_\eta^2\psi+
(\alpha+\beta|\psi|^2)\psi=0}.
$$

In particular $\eta=1$ gives the requested equation. Its conjugate follows from variation in $\psi$.

For variation in $A$, $\delta D_\eta\psi=-i\eta q_s\delta A\,\psi/\hbar$. The kinetic variation is $-j_\eta\cdot\delta A$, where

$$
j_\eta=\frac{\eta q_s\hbar}{m_s}\operatorname{Im}(\psi^*\nabla\psi)
-\frac{q_s^2}{m_s}|\psi|^2A.
$$

The magnetic variation is $(\nabla\times B)\cdot\delta A/\mu_0$ after [integration by parts](../../../../../integration-by-parts.md). Therefore

$$
\boxed{\nabla\times B=\mu_0j_\eta}.
$$

For $\eta=1$ this current equals the two displayed forms in the question. For the literal plus-sign [energy](../../../../../energy.md), $\eta=-1$, the phase-gradient current term has the opposite sign and the field equation contains $D_{-1}^2$. Thus the requested set follows after correcting that one [energy](../../../../../energy.md) sign, not from silently varying inconsistent expressions. This is the [gauge-coupling sign in Ginzburg-Landau superconductivity](../../../../../gauge-coupling-sign-in-ginzburg-landau-superconductivity.md).

Now use the intended convention and write $\psi=\sqrt{n_s}e^{i\theta}$ with $n_s>0$. Dividing $D_1\psi=0$ by $\psi$ separates real and imaginary parts:

$$
\nabla\sqrt{n_s}=0,\qquad
\boxed{\hbar\nabla\theta=q_sA}.
$$

Thus $n_s$ is constant on each [connected](../../../../../connected-space.md) region. The remaining field equation requires $\alpha+\beta n_s=0$, so for $T<T_c$,

$$
\boxed{n_s=-\alpha/\beta>0}.
$$

The current is $j=(q_sn_s/m_s)(\hbar\nabla\theta-q_sA)=0$. Taking the curl locally gives $B=0$, hence also solves the Maxwell equation.

For a closed curve on which the [order parameter](../../../../../order-parameter.md) is nonzero and $D_1\psi=0$, Stokes' theorem gives

$$
\Phi=\oint_C A\cdot dl=\frac{\hbar}{q_s}\oint_C\nabla\theta\cdot dl
=\frac{\hbar}{q_s}[\theta]_C.
$$

Single-valuedness of $\psi$ permits phase change $2\pi N$, so the flux quantum magnitude is $h/|q_s|$ (for Cooper pairs, $h/(2|e|)$). There is an important geometric qualification: if the entire spanning surface lies in the smooth zero-field superconducting region assumed above, its flux and the total boundary winding are zero. Nonzero quantized flux occurs through a hole or vortex core where those assumptions do not hold over the spanning surface. More generally, without $j=0$ along the curve, the exact quantized quantity is the fluxoid

$$
\boxed{\oint_C\left(A+\frac{m_s}{q_s^2n_s}j\right)\cdot dl
=\frac h{q_s}N}.
$$

Thus [fluxoid and flux quantization in a superconductor](../../../../../fluxoid-and-flux-quantization-in-a-superconductor.md) are related but are not interchangeable without the current condition.

## ↑ Ancestors (10)

1. [35B](../35b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
