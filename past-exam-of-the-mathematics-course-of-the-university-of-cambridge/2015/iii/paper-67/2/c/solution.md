<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Part (a) shows that $\mathcal L$ is invariant throughout the interpolation. As the Hamiltonians are Hermitian, $\mathcal L^\perp$ is invariant as well: evolution starting in $\mathcal L$ has no leakage into other sectors. The [quantum adiabatic theorem](../../../../../../adiabatic-theorem.md) may therefore be applied using the restricted [spectral gap](../../../../../../spectral-gap.md), even if other sectors of the full Hamiltonian have different low-energy levels.

Combining (b)(iv) with the supplied bound for $s>1/3$ gives $\min_s\Delta(M(s))\geq c/(T+1)^2$ for a constant $c>0$. The matrix $E-D$ has diagonal entries $1/2,0,\ldots,0,-1/2$ and off-diagonal entries $-1/2$. Its [Gershgorin discs](../../../../../../gershgorin-disc.md) all lie in $[-1,1]$, so $\|E-D\|\leq1$. Thus the runtime criterion for [adiabatic preparation of a computational history state](../../../../../../adiabatic-preparation-of-a-computational-history-state.md) is satisfied by

$$
\boxed{\tau=O\!\left(\frac{(T+1)^6}{\epsilon}\right)}
$$

with a sufficiently large constant.

Starting from the supplied initial [ground state](../../../../../../ground-state.md) $|e_0\rangle$, the resulting state $\rho_{\rm out}$ obeys

$$
\boxed{\|\rho_{\rm out}-|\varphi\rangle\langle\varphi|\|_1\leq\epsilon.}
$$

Here the trace norm follows the question's convention; the conventional [trace distance](../../../../../../trace-distance.md) is half this norm. The Hamiltonian has $O(T)$ explicitly specified terms, each acting on at most five [qubits](../../../../../../qubit.md), so its description and the runtime are polynomial in circuit size. If $\epsilon^{-1}$ is polynomially bounded, the whole preparation has polynomial cost. The initial computational input is assumed to have been prepared, as in the premise of the [quantum adiabatic theorem](../../../../../../adiabatic-theorem.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
