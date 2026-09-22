<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Bell basis](../../../../../../bell-basis.md) consists of

$$
|\Phi^\pm\rangle=\frac{|00\rangle\pm|11\rangle}{\sqrt2},\qquad
|\Psi^\pm\rangle=\frac{|01\rangle\pm|10\rangle}{\sqrt2}.
$$

Let $Z=\sigma_z$, $X=\sigma_x$. The [Pauli operators](../../../../../../pauli-operator.md) $Z\otimes Z$ and $X\otimes X$ commute: each of the two local anticommutations contributes a minus sign, so they cancel. Their eigenvalue table is

$$
\begin{array}{c|cc|cc}
\text{state}&Z\otimes Z&X\otimes X&\text{parity bit}&\text{phase bit}\\\hline
\Phi^+&+1&+1&0&0\\
\Phi^-&+1&-1&0&1\\
\Psi^+&-1&+1&1&0\\
\Psi^-&-1&-1&1&1
\end{array}
$$

To make the bit values literally zero or one rather than signed eigenvalues, the commuting [Bell parity and phase observables](../../../../../../bell-parity-and-phase-observables.md) are

$$
\boxed{B_{\rm parity}=\frac{I-Z\otimes Z}{2},\qquad
B_{\rm phase}=\frac{I-X\otimes X}{2}.}
$$

They distinguish all four states jointly. The parity bit records whether the computational bits agree; the phase bit records the relative sign.

## ↑ Ancestors (11)

1. [I](../i.md)
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
