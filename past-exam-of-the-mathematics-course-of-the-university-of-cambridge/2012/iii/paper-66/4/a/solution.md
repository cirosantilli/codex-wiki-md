<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

All time-dependent [Hamiltonian operators](../../../../../../hamiltonian-quantum-mechanics.md) are multiples of the same fixed operator, so they commute and their [time-ordered exponential](../../../../../../time-ordered-exponential.md) reduces to an ordinary exponential. Let $P_1=(I-Z_S)/2$. With $\hbar=1$ and the given unit coupling integral,

$$
U=\exp\left[-\frac{i\pi}{2}P_1\otimes(I-X_D)\right]
=P_0\otimes I+P_1\otimes e^{-i\pi(I-X_D)/2}.
$$

Since $X_D^2=I$,

$$
e^{-i\pi(I-X_D)/2}
=e^{-i\pi/2}\left[\cos(\pi/2)I+i\sin(\pi/2)X_D\right]=X_D.
$$

Thus

$$
\boxed{U=P_0\otimes I+P_1\otimes X_D,\qquad
U|s,d\rangle=|s,d\oplus s\rangle.}
$$

It is exactly the [CNOT gate](../../../../../../controlled-not-gate.md) with $S$ controlling $D$, with no residual relative phase. Acting on $(c_0|0\rangle+c_1|1\rangle)_S|0\rangle_D$ correlates the system basis label with the apparatus label, producing $c_0|00\rangle+c_1|11\rangle$ as required.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
