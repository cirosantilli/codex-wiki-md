<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The requested [energy eigenvalue](../../../../../energy-eigenvalue-split.md) is $E_2$. By the [Born rule](../../../../../born-rule.md), its [probability amplitude](../../../../../probability-amplitude.md) is the [inner product](../../../../../inner-product-split.md) $c_2=\langle\psi_2,\Psi(0)\rangle$. Put $u=\pi x/a$ and use $e^{iu}\sin u=\tfrac12\sin2u+i\sin^2u$:

$$
c_2=\frac2\pi\int_0^\pi\sin2u\,e^{iu}\sin u\,du=\frac1\pi\int_0^\pi\sin^22u\,du+\frac{2i}\pi\int_0^\pi\sin2u\sin^2u\,du=\frac12.
$$

The first integral is $\pi/2$; the second is zero under $u\mapsto\pi-u$. Therefore

$$
\boxed{\Pr(E=E_2)=|c_2|^2=\frac14.}
$$

For the time-independent [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), expand in its [orthonormal basis](../../../../../orthonormal-basis.md) of [energy eigenstates](../../../../../energy-eigenstate.md):

$$
\Psi(x,t)=\sum_{n\geq1}c_n e^{-iE_nt/\hbar}\psi_n(x).
$$

[Unitary time evolution](../../../../../unitary-time-evolution.md) changes $c_2$ to $c_2e^{-iE_2t/\hbar}$, whose modulus is unchanged. Thus the same [energy measurement](../../../../../energy-measurement.md) [probability](../../../../../probability.md) holds at every time, even though relative [quantum phases](../../../../../quantum-phase.md) and other measurements can change.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
