<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret the imposed measurement restriction as direct measurement of the encoded two-qubit [Bell state](../../../../bell-state-split.md) in the [computational basis](../../../../computational-basis.md), without a preceding entangling Bell decoder. For the uniform messages the conditional probabilities are

$$
\begin{array}{c|cccc}
&00&01&10&11\\\hline
\Psi^+&0&1/2&1/2&0\\
\Psi^-&0&1/2&1/2&0\\
\Phi^+&1/2&0&0&1/2\\
\Phi^-&1/2&0&0&1/2
\end{array}.
$$

Each outcome has probability $1/4$, so $H(Y)=2$ bits, while $H(Y|X)=1$ bit. Therefore

$$
\boxed{I(X:Y)=1\ \text{bit}.}
$$

The outcome reveals even versus odd parity, but none of the plus/minus label. Each outcome is compatible with two equally probable messages.

Now insert an arbitrary single-qubit [unitary operator](../../../../unitary-operator.md) $U$ on one wire immediately before measurement. Measuring that wire is equivalent to measuring along a [Bloch vector](../../../../bloch-vector.md) $\boldsymbol n$, with the other wire still measured along $z$. All four [Bell states](../../../../bell-state-split.md) have zero local means, and $\langle X\otimes Z\rangle=\langle Y\otimes Z\rangle=0$, whereas $\langle Z\otimes Z\rangle=+1$ for $\Phi^\pm$ and $-1$ for $\Psi^\pm$. Hence

$$
\Pr(r,s\mid\Phi^\pm)=\tfrac14(1+rsn_z),\qquad
\Pr(r,s\mid\Psi^\pm)=\tfrac14(1-rsn_z),\qquad r,s=\pm1.
$$

The sign within each pair is still inaccessible, and

$$
\boxed{I_U(X:Y)=1-h_2\left(\frac{1+n_z}{2}\right)\leq1.}
$$

It stays one for a computational-axis measurement, but a [Hadamard gate](../../../../hadamard-gate.md) makes $n_z=0$ and reduces it to zero. Thus a single local gate can change the information, by reducing it, and cannot increase it above one bit.

There is an important scope qualification: if Bob is allowed the full two-qubit decoder from part b before his final computational measurement, those measurements already identify all four messages and give two bits. The one-bit result refers to restricting the Bell readout itself to product computational measurements. Merely specifying the final detector basis without restricting the decoder would not impose that one-bit limit.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
