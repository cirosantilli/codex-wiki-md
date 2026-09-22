<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $N=2^t$ and write $U|u\rangle=e^{i\phi}|u\rangle$, with $|u\rangle$ normalized. The [Hadamard gates](../../../../../../hadamard-gate.md) prepare the control register in $N^{-1/2}\sum_{k=0}^{N-1}|k\rangle$. Controlled powers of the [unitary operator](../../../../../../unitary-operator.md) then give [quantum phase kickback](../../../../../../phase-kickback.md):

$$
|k\rangle|u\rangle\longmapsto|k\rangle U^k|u\rangle=e^{ik\phi}|k\rangle|u\rangle.
$$

Thus the register [quantum state](../../../../../../quantum-state.md) is $N^{-1/2}\sum_k e^{ik\phi}|k\rangle$, while the target remains $|u\rangle$. Define the [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) by $F_N|m\rangle=N^{-1/2}\sum_k e^{2\pi ikm/N}|k\rangle$. Its inverse gives

$$
\frac1N\sum_{m=0}^{N-1}\left(\sum_{k=0}^{N-1}e^{ik(\phi-2\pi m/N)}\right)|m\rangle.
$$

When $\phi=2\pi n/N$, the inner [finite geometric series](../../../../../../finite-geometric-series.md) equals $N$ if $m\equiv n\pmod N$ and zero otherwise. Therefore [exact quantum phase estimation](../../../../../../exact-quantum-phase-estimation.md) gives

$$
\boxed{m=n\bmod N\quad\text{with probability one},\qquad \widehat\phi=\frac{2\pi m}{N}\pmod{2\pi}.}
$$

The [quantum phase](../../../../../../quantum-phase.md), rather than an unrestricted integer $n$, is recovered modulo $2\pi$.

The printed circuit has no bit-reversal swaps. Its top control uses $U^{2^{t-1}}$, and its measured top wire gives the least significant output bit. Write $n\bmod N=\sum_{j=0}^{t-1}2^jb_j$. Before the top wire's final [Hadamard gate](../../../../../../hadamard-gate.md), its relative [quantum phase](../../../../../../quantum-phase.md) is $2^{t-1}\phi=\pi n$, so that gate produces $b_0$. The controlled inverse [quantum phase](../../../../../../quantum-phase.md) gates then subtract its contribution from lower wires. More generally, before the final [Hadamard gate](../../../../../../hadamard-gate.md) on wire $j$, the relative [quantum phase](../../../../../../quantum-phase.md) is

$$
\frac{2\pi}{2^{j+1}}\left(n-\sum_{h=0}^{j-1}2^hb_h\right)=\pi b_j\pmod{2\pi},
$$

so that wire gives $b_j$ deterministically. For the three-wire drawing, the correct interpretation is

$$
\boxed{n\bmod8=j_0+2j_1+4j_2.}
$$

Equivalently, its Fourier-inversion circuit is $R F_N^\dagger$, where $R$ reverses the register bits. Relabeling the measured bits or appending swaps gives the usual integer output. This bit convention matters, for example, when [quantum phase](../../../../../../quantum-phase.md) $\pi$ produces top-to-bottom bits $001$, representing the label four rather than one.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
