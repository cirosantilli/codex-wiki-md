<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use a mostly-plus target [metric tensor](../../../../../metric-tensor.md) and the standard [open-string mode expansion](../../../../../open-string-mode-expansion.md) convention $\alpha_0^\mu=\sqrt{2\alpha'}p^\mu$. The [integer string oscillator level](../../../../../integer-string-oscillator-level.md) is $N=\sum_{n\ge1}\alpha_{-n}\cdot\alpha_n$, whose [eigenvalues](../../../../../eigenvalue.md) are nonnegative integers. Then $L_0=N+\alpha'p^2$, so the [string mass-shell condition](../../../../../string-mass-shell-condition.md) gives

$$
\boxed{M^2=-p^2=\frac{N-1}{\alpha'}.}
$$

The ground state is a [tachyon](../../../../../tachyon.md), and the level-one state is massless. The [physical string state](../../../../../physical-string-state.md) conditions in [old covariant string quantization](../../../../../old-covariant-string-quantization.md) are

$$
(L_0-1)|\psi\rangle=0,\qquad L_m|\psi\rangle=0\quad(m>0).
$$

Only the positive-mode [Virasoro constraints](../../../../../virasoro-constraint.md) annihilate a ket; their negative-mode partners annihilate the corresponding bra. Imposing both signs on every ket would contradict the nonzero [Virasoro central extension](../../../../../virasoro-central-extension.md).

The [central charge](../../../../../central-charge.md) comes from [normal ordering](../../../../../normal-ordering.md) the quadratic oscillator expressions. Classically their [Poisson brackets](../../../../../poisson-bracket.md) have no central term. Quantum mechanically, moving [annihilation operators](../../../../../annihilation-operator.md) through [creation operators](../../../../../creation-operator.md) produces double contractions. From the oscillator [commutator](../../../../../commutator.md) one obtains $[L_m,\alpha_n^\mu]=-n\alpha_{m+n}^\mu$, which gives the noncentral part $(m-n)L_{m+n}$.

The coefficient is fixed by the [free-boson Virasoro central term](../../../../../free-boson-virasoro-central-term.md). On a formal zero-momentum vacuum, for $m>0$,

$$
L_{-m}|0\rangle=\frac12\sum_{r=1}^{m-1}\alpha_{-(m-r)}\cdot\alpha_{-r}|0\rangle.
$$

The two contraction pairings give

$$
\langle0|L_mL_{-m}|0\rangle=\frac D2\sum_{r=1}^{m-1}r(m-r)=\frac D{12}m(m^2-1).
$$

Here $\eta_{\mu\nu}\eta^{\mu\nu}=D$; the time coordinate contributes one, just as each spatial coordinate does. Comparing with the [Virasoro algebra](../../../../../virasoro-algebra.md) proves

$$
\boxed{c_{\rm matter}=D.}
$$

This counts covariant target coordinates. It is distinct from the $D-2$ physical transverse polarizations. Including the [central charge of reparameterization ghosts](../../../../../central-charge-of-reparameterization-ghosts.md) gives $c_{\rm total}=D-26$; cancellation of the [worldsheet Weyl anomaly](../../../../../worldsheet-weyl-anomaly.md) gives the usual [critical dimension of the bosonic string](../../../../../critical-dimension-of-string-theory.md) $D=26$.

A general level-one state is

$$
|\epsilon;k\rangle=\epsilon_\mu\alpha_{-1}^\mu|0;k\rangle.
$$

The zero-mode constraint requires $k^2=0$. Since $[L_1,\alpha_{-1}^\mu]=\alpha_0^\mu$, the remaining nontrivial positive-mode constraint is $k\cdot\epsilon=0$; all $L_m$ with $m\ge2$ act trivially at this level. Thus the [polarization vector](../../../../../polarization-vector.md) is transverse to a nonzero null momentum.

There is also a [null string state](../../../../../null-string-state.md) $L_{-1}|0;k\rangle=\sqrt{2\alpha'}\,k\cdot\alpha_{-1}|0;k\rangle$. It is physical when $k^2=0$ and orthogonal to every physical polarization. The [null-state quotient of a string](../../../../../null-state-quotient-of-a-string.md) therefore identifies

$$
\epsilon\sim\epsilon+\lambda k.
$$

Choose $k=(E,E,0,\ldots,0)$. Transversality sets $\epsilon^1=\epsilon^0$, and the null-state identification removes this common component. The remaining $D-2$ spatial components have positive norm. Hence **the physical level-one states form a massless vector with $D-2$ polarizations**, or 24 at the critical dimension. The removed component is gauge redundancy. States violating the constraints, including independent timelike negative-norm polarizations, are unphysical; physical null states are removed by the quotient rather than counted as additional particles.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
