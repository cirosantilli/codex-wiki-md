<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose the phase convention in the question and use the [gauge covariant derivative](../../../../../../gauge-covariant-derivative.md) $D_\mu=\partial_\mu+ieA_\mu$. For a charged [Dirac field](../../../../../../dirac-field.md), the [quantum electrodynamics](../../../../../../quantum-electrodynamics.md) Lagrangian is

$$
\mathcal L=-\frac14F_{\mu\nu}F^{\mu\nu}+\bar\psi(i\gamma^\mu D_\mu-m)\psi,
\qquad F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu.
$$

The simultaneous local [gauge transformation](../../../../../../gauge-transformation.md) is

$$
\boxed{\psi'=e^{ie\chi}\psi,\qquad
\bar\psi'=\bar\psi e^{-ie\chi},\qquad A'_\mu=A_\mu-\partial_\mu\chi}.
$$

Direct differentiation gives $D'_\mu\psi'=e^{ie\chi}D_\mu\psi$: the derivative of the phase cancels the shift of $A_\mu$. The mass term and covariant kinetic term are therefore invariant. The [electromagnetic field tensor](../../../../../../electromagnetic-field-tensor.md) is unchanged because mixed partial derivatives of $\chi$ commute. This proves classical [gauge invariance](../../../../../../gauge-invariance.md) of the coupled field action. A charged scalar similarly uses $(D_\mu\phi)^*D^\mu\phi$ and a potential depending only on $|\phi|^2$.

The electromagnetic coupling is $-eA_\mu\bar\psi\gamma^\mu\psi$. The matter equations give a conserved current $j^\mu=e\bar\psi\gamma^\mu\psi$, with $\partial_\mu j^\mu=0$. Constant $\chi$ gives the global symmetry and its conserved charge. When applying [Noether's theorem](../../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md), the sign of the parameterized Noether generator can be reversed without changing this conservation law; the transformation and coupling signs above remain fixed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
