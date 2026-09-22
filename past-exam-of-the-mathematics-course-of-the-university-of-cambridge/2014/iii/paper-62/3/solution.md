<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $U_1=e^{-iH(t-t_1)/\hbar}$ and $U_2=e^{-iH(t_2-t)/\hbar}$ describe [unitary time evolution](../../../../../unitary-time-evolution.md). For an ideal [projective measurement](../../../../../projective-measurement.md) with the [Lüders rule](../../../../../luders-rule.md), its unconditioned outcome probability is $p_j=\|P_jU_1|\psi\rangle\|^2$. After that outcome, the normalized state is $P_jU_1|\psi\rangle/\sqrt{p_j}$. The [Born rule](../../../../../born-rule.md) probability of successful [postselection](../../../../../postselection.md) is then $|\langle\psi'|U_2P_jU_1|\psi\rangle|^2/p_j$. Multiplying gives the joint probability

$$
\Pr(j,\psi'\mid\psi)=|\langle\psi'|U_2P_jU_1|\psi\rangle|^2.
$$

[Conditional probability](../../../../../conditional-probability.md) therefore gives the [Aharonov-Bergmann-Lebowitz rule](../../../../../aharonov-bergmann-lebowitz-rule.md):

$$
\boxed{\Pr(j\mid\psi,\psi',\{P_k\})=
\frac{|\langle\psi'|U_2P_jU_1|\psi\rangle|^2}
{\sum_k|\langle\psi'|U_2P_kU_1|\psi\rangle|^2}.}
$$

The denominator must be positive; otherwise the selected subensemble does not occur. Define the forward-evolved ket $|a\rangle=U_1|\psi\rangle$ and backward-evolved ket $|b\rangle=U_2^\dagger|\psi'\rangle$. The numerator becomes $|\langle b|P_j|a\rangle|^2$, which is unchanged by interchanging $a,b$. Equivalently, with $\rho_a=|a\rangle\langle a|$ and $\rho_b=|b\rangle\langle b|$,

$$
\Pr(j\mid a,b)=\frac{\operatorname{Tr}(\rho_bP_j\rho_aP_j)}{\sum_k\operatorname{Tr}(\rho_bP_k\rho_aP_k)}.
$$

This expresses the boundary-state symmetry explicitly. It follows from the ordinary time-asymmetric preparation, [Born rule](../../../../../born-rule.md), and state update; it does not posit an additional backward dynamical collapse.

Restore the post-selected vector omitted entirely from the TeX aid by reading the original PDF. Write $D=N^2-N+1$ and

$$
|\psi'\rangle=\frac{\sum_{i=1}^N|i\rangle-(N-1)|N+1\rangle}{\sqrt D}.
$$

Its norm is one because $N+(N-1)^2=D$. For the uniform prestate and $H=0$, put $c=1/\sqrt{(N+1)D}$. The individual transition amplitudes are

$$
\langle\psi'|P_i|\psi\rangle=c\quad(1\leq i\leq N),\qquad
\langle\psi'|P_{N+1}|\psi\rangle=-(N-1)c,
\qquad \langle\psi'|\psi\rangle=c.
$$

In experiment $E_i$, the complement amplitude is $c-c=0$. Thus for every $i\leq N$,

$$
\boxed{\Pr(P_i\mid E_i,\psi,\psi')=1,\qquad
\Pr(I-P_i\mid E_i,\psi,\psi')=0.}
$$

The successful [postselection](../../../../../postselection.md) rate in this experiment is $c^2=1/((N+1)D)$.

In the fully resolved experiment $E_0$, the [ABL rule](../../../../../aharonov-bergmann-lebowitz-rule.md) squares the individual amplitudes before summing. Their squared sum is $Dc^2=1/(N+1)$, giving

$$
\boxed{\Pr(P_i\mid E_0,\psi,\psi')=\frac1D\quad(1\leq i\leq N),\qquad
\Pr(P_{N+1}\mid E_0,\psi,\psi')=\frac{(N-1)^2}{D}.}
$$

These probabilities sum to one. For $N=1$ they reduce to a single certain outcome in either [measurement in quantum mechanics](../../../../../quantum-measurement-split.md). For $N\geq2$, the [N-box pre- and post-selection paradox](../../../../../n-box-pre-and-post-selection-paradox.md) is that each separate binary question can be answered affirmatively with certainty, although the fully resolved [measurement in quantum mechanics](../../../../../quantum-measurement-split.md) cannot give all those outcomes at once.

There is no inconsistency. In $E_i$, the unresolved complement preserves coherent cancellation between its basis contributions under the [Lüders rule](../../../../../luders-rule.md). In $E_0$, those alternatives are resolved, so their squared amplitudes add instead. The different [projective measurements](../../../../../projective-measurement.md) disturb the state differently and have different [postselection](../../../../../postselection.md) success rates. Merely merging the recorded $E_0$ outcomes afterwards does not reproduce $E_i$. This is the [context dependence of pre- and post-selected measurements](../../../../../context-dependence-of-pre-and-post-selected-measurements.md); certainties in mutually alternative experiments do not describe simultaneous measurement-independent properties.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
