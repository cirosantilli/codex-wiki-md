<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the conventional [phase gate](../../../../phase-gate.md) $P_\varphi=\operatorname{diag}(1,e^{i\varphi})$ in [computational basis](../../../../computational-basis.md) order $0,1$. The single-qubit [Hadamard gate](../../../../hadamard-gate.md) and the successive [quantum states](../../../../quantum-state.md) are

$$
\boxed{H=\frac1{\sqrt2}\begin{pmatrix}1&1\\1&-1\end{pmatrix},}
\qquad
|0\rangle\xrightarrow{H}\frac{|0\rangle+|1\rangle}{\sqrt2}
\xrightarrow{P_\varphi}\frac{|0\rangle+e^{i\varphi}|1\rangle}{\sqrt2}.
$$

The final [Hadamard gate](../../../../hadamard-gate.md) recombines the two components, giving

$$
\boxed{|\psi_{\rm out}\rangle=
\frac{1+e^{i\varphi}}2|0\rangle+\frac{1-e^{i\varphi}}2|1\rangle
=e^{i\varphi/2}\left(\cos\frac\varphi2|0\rangle-i\sin\frac\varphi2|1\rangle\right).}
$$

The leading factor in the last expression is a [global phase](../../../../global-phase.md). The [Born rule](../../../../born-rule.md) therefore yields

$$
\boxed{P_0(\varphi)=\left|\frac{1+e^{i\varphi}}2\right|^2
=\frac{1+\cos\varphi}{2}=\cos^2\frac\varphi2.}
$$

At $\varphi=0$ the output is certainly zero, whereas at $\varphi=\pi$ it is certainly one. The [phase gate](../../../../phase-gate.md) changes no intermediate outcome [probabilities](../../../../probability.md); the final [Hadamard gate](../../../../hadamard-gate.md) converts a relative [quantum phase](../../../../quantum-phase.md) into an observable [quantum interference](../../../../quantum-interference.md) fringe.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
