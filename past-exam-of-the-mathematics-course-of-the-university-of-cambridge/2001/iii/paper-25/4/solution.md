<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

On an $N$-dimensional register, the [quantum Fourier transform](../../../../../quantum-fourier-transform.md) with positive-exponent convention is

$$
\boxed{F_N|x\rangle=\frac1{\sqrt N}\sum_{y=0}^{N-1}e^{2\pi ixy/N}|y\rangle.}
$$

It is the unitary version of the [discrete Fourier transform](../../../../../discrete-fourier-transform.md) on amplitudes. The inner product of columns $x,x'$ is $N^{-1}\sum_y e^{2\pi i(x'-x)y/N}$, equal to one when $x=x'$ and zero otherwise by a finite [geometric series](../../../../../geometric-series.md), so the transformation is unitary.

For the qubit implementation take $N=2^n$, write $x=x_1\cdots x_n$ in most-significant-bit-first order, and put $0.x_j\cdots x_n=\sum_{l=j}^n x_l2^{-(l-j+1)}$. Expanding $y=\sum_jy_j2^{n-j}$ separates the Fourier phase as a product. The resulting [dyadic quantum Fourier transform circuit](../../../../../dyadic-quantum-fourier-transform-circuit.md) identity is

$$
\boxed{F_{2^n}|x_1\cdots x_n\rangle=
\frac{|0\rangle+e^{2\pi i0.x_n}|1\rangle}{\sqrt2}
\otimes\frac{|0\rangle+e^{2\pi i0.x_{n-1}x_n}|1\rangle}{\sqrt2}
\otimes\cdots\otimes
\frac{|0\rangle+e^{2\pi i0.x_1\cdots x_n}|1\rangle}{\sqrt2}.}
$$

Indeed the phase on output bit $y_j$ is $e^{2\pi ixy_j/2^j}$, depending on the last $j$ input bits; multiplying the factors recovers $e^{2\pi ixy/2^n}$ and the normalization $2^{-n/2}$.

Implement the product in reverse wire order as follows. Process input wire $j$, starting at $j=1$. A [Hadamard gate](../../../../../hadamard-gate.md) maps $|x_j\rangle$ to $(|0\rangle+e^{2\pi i x_j/2}|1\rangle)/\sqrt2$. For each still-unprocessed wire $l>j$, apply a [controlled phase gate](../../../../../controlled-phase-gate.md) with control $l$, target $j$, and target phase

$$
R_{l-j+1}=\operatorname{diag}\left(1,e^{2\pi i/2^{l-j+1}}\right).
$$

On a computational-basis input this multiplies the target's one-component by $e^{2\pi i x_l/2^{l-j+1}}$, so the processed wire becomes exactly $(|0\rangle+e^{2\pi i0.x_j\cdots x_n}|1\rangle)/\sqrt2$. Continue through all wires and reverse their order using [SWAP gates](../../../../../swap-gate.md). This equals the boxed transform on every basis vector and therefore on arbitrary superpositions by linearity; it does not require learning the input bits by measurement.

There are **$\boxed{n\text{ Hadamards},\quad n(n-1)/2\text{ controlled phase gates},\quad\lfloor n/2\rfloor\text{ swaps}}$**. A swap is three [controlled-NOT gates](../../../../../controlled-not-gate.md), since the alternating control directions send $(a,b)$ successively to $(a,a\oplus b)$, then $(b,a\oplus b)$, and finally $(b,a)$. Thus the exact transform uses $O(n^2)$ one- and two-qubit gates from this phase-gate family, polynomial in the register size $n=\log_2N$. This is a circuit-complexity statement, not a claim that all $N$ transformed amplitudes can be read out efficiently. If a fixed finite gate alphabet is required, the phase rotations must instead be synthesized to the desired accuracy; the exact count treats them as the available simple rotation gates.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
