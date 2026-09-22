<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply a [Hadamard gate](../../../../../../hadamard-gate.md) to qubit $A$, followed by a [controlled-NOT gate](../../../../../../controlled-not-gate.md) with $A$ controlling $B$. The resulting [Bell-basis conversion circuit](../../../../../../bell-basis-conversion-circuit.md) is $U=\operatorname{CNOT}(H\otimes I)$ and gives

$$
U|ij\rangle=\frac{|0j\rangle+(-1)^i|1,j\oplus1\rangle}{\sqrt2}.
$$

Thus $00,01,10,11$ map respectively to $\Phi^+,\Psi^+,\Phi^-,\Psi^-$. The first input bit becomes the phase bit and the second becomes the parity bit.

Both gates are self-inverse, but inversion of their product reverses the order:

$$
\boxed{U^{-1}=U^\dagger=(H\otimes I)\operatorname{CNOT}.}
$$

So **the same two gates convert the [Bell basis](../../../../../../bell-basis.md) back to the [computational basis](../../../../../../computational-basis.md) when applied in reverse order**: first the controlled-NOT, then the Hadamard. Using the forward order twice does not generally work, since these gates do not commute. For example, $U|\Phi^+\rangle=(|00\rangle+|01\rangle-|10\rangle+|11\rangle)/2$, which is not a computational-basis state.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
