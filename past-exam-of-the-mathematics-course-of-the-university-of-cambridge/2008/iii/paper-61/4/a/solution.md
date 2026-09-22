<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The feedback law printed in the PDF is not sufficient for the asserted monotonicity. We first derive the exact identity, then give a counterexample and the corrected law. Both [density operators](../../../../../../density-matrix.md) evolve unitarily, so $\operatorname{Tr}\rho^2$ and $\operatorname{Tr}\rho_d^2$ are constant. Thus

$$
V=\|\rho-\rho_d\|_{\rm HS}^2=\operatorname{Tr}\rho^2+\operatorname{Tr}\rho_d^2-2\operatorname{Tr}(\rho_d\rho).
$$

Cyclicity of the [trace](../../../../../../matrix-trace.md) gives $\operatorname{Tr}([-iH_0,\rho_d]\rho)=-\operatorname{Tr}(\rho_d[-iH_0,\rho])$. These drift terms cancel in the [derivative](../../../../../../derivative.md) of the overlap, leaving

$$
\frac d{dt}\operatorname{Tr}(\rho_d\rho)=fC,\qquad
C=\operatorname{Tr}(\rho_d[-iH_1,\rho]),\qquad
\boxed{\dot V=-2fC.}
$$

Here $C$ is real: $-i[H_1,\rho]$ is Hermitian, and the [trace](../../../../../../matrix-trace.md) of the product of two [Hermitian matrices](../../../../../../hermitian-operator.md) is real. This is the [Hilbert-Schmidt Lyapunov feedback identity](../../../../../../hilbert-schmidt-lyapunov-feedback-identity.md).

For a direct counterexample to the source's overlap law, take $H_0=0$, $H_1=\sigma_y/2$, $\rho_d=(I+\sigma_z)/2$ and $\rho=(I+\sigma_x)/2$. All are admissible qubit operators and states. The printed overlap is $f=\operatorname{Tr}(\rho_d\rho)=1/2$, but $-i[H_1,\rho]=-\sigma_z/2$ gives $C=-1/2$. Hence $\dot V=1/2>0$: the distance initially increases. This proves that [feedback based on state overlap need not be stabilizing](../../../../../../feedback-based-on-state-overlap-need-not-be-stabilizing.md).

The intended [Lyapunov quantum control](../../../../../../lyapunov-quantum-control.md) replaces the overlap by its control-direction [derivative](../../../../../../derivative.md):

$$
\boxed{f=k\operatorname{Tr}(\rho_d[-iH_1,\rho]),\quad k>0,
\qquad\dot V=-2kC^2\leq0.}
$$

The conclusion is nonincrease, not strict decrease or automatic convergence. For example, opposite computational-basis [pure states](../../../../../../pure-state.md), diagonal $H_0$, and $H_1=\sigma_x$ give $C=0$ and zero control even though $V=2$. Target convergence requires further invariant-set and reachability conditions. A target with a different spectrum is also inaccessible under [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md) evolution. The density-operator [derivatives](../../../../../../derivative.md) in the governing equations use the dots visible in the PDF, which the TeX loses.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
