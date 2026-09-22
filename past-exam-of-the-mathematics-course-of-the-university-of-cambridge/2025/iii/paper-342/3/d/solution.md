<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $a=\gamma_{2M}$ and $b=\gamma_{2M-1}$. The ancilla condition $iab|\psi\rangle=|\psi\rangle$ implies $a|\psi\rangle=ib|\psi\rangle$ and lets every occurrence of $a$ on the state be replaced by $ib$. Define the two parity projectors

$$
P_1=\frac{1-i\gamma_3b}{2},
\qquad
P_2=\frac{1+\gamma_1\gamma_2\gamma_4b}{2}.
$$

Their factors square to one, so they are valid [fermion-parity measurement](../../../../../../fermion-parity-measurement.md) projectors. Expanding $P_1P_2$, using the Majorana anticommutation relations, replacing $a$ with $ib$ on $|\psi\rangle$, and using

$$
e^{\pi\gamma_3a/4}=\frac{1+\gamma_3a}{\sqrt2},
\qquad
e^{i\pi\gamma_1\gamma_2\gamma_3\gamma_4/4}
=\frac{1+i\gamma_1\gamma_2\gamma_3\gamma_4}{\sqrt2},
$$

gives

$$
\boxed{
e^{i\pi\gamma_1\gamma_2\gamma_3\gamma_4/4}|\psi\rangle
\propto
e^{\pi\gamma_3\gamma_{2M}/4}
\frac{1-i\gamma_3\gamma_{2M-1}}2
\frac{1+\gamma_1\gamma_2\gamma_4\gamma_{2M-1}}2
|\psi\rangle.}
$$

The proportionality absorbs the probability amplitude for obtaining the two displayed measurement outcomes. This realizes the four-Majorana phase gate using one braid and parity measurements.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
