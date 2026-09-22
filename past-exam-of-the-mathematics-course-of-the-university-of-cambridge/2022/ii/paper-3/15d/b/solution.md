<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the convention

$$
\operatorname{QFT}_N|k\rangle
=\frac1{\sqrt N}\sum_{j=0}^{N-1}e^{2\pi ijk/N}|j\rangle.
$$

Changing the summation variable from $j$ to $j-1$ gives

$$
S\operatorname{QFT}_N|k\rangle
=e^{-2\pi ik/N}\operatorname{QFT}_N|k\rangle.
$$

Thus the Fourier-basis states are [eigenvectors](../../../../../../eigenvector.md) of the cyclic shift, with respective [eigenvalues](../../../../../../eigenvalue.md) $e^{-2\pi ik/N}$, and the [cyclic shift diagonalization by the quantum Fourier transform](../../../../../../cyclic-shift-diagonalization-by-the-quantum-fourier-transform.md) is

$$
S=\operatorname{QFT}_N D\operatorname{QFT}_N^{-1},
\qquad
D|k\rangle=e^{-2\pi ik/N}|k\rangle.
$$

For $N=4$, write $k=2x+y$ with $x,y\in\{0,1\}$. Then

$$
e^{-2\pi ik/4}=e^{-i\pi x}e^{-i\pi y/2},
$$

so

$$
D=P(-\pi)\otimes P(-\pi/2),
\qquad
P(\theta)=\begin{pmatrix}1&0\\0&e^{i\theta}\end{pmatrix}.
$$

Hence the required [quantum circuit](../../../../../../quantum-circuit-split.md) applies, from input to output,

$$
\boxed{
\operatorname{QFT}_4^{-1}
\;\longrightarrow\;
P(-\pi)\otimes P(-\pi/2)
\;\longrightarrow\;
\operatorname{QFT}_4
}.
$$

The first phase gate acts on the most significant qubit $x$ and the second on the least significant qubit $y$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
