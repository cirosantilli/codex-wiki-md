<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $|+\rangle=(|0\rangle+|1\rangle)/\sqrt2$. Before any interaction the system is in the [pure state](../../../../../../pure-state.md) $|\psi_S\rangle=\alpha|0\rangle+\beta|1\rangle$, so

$$
\rho_S^{(0)}=
\begin{pmatrix}
|\alpha|^2&\alpha\beta^*\\
\alpha^*\beta&|\beta|^2
\end{pmatrix}.
$$

One interaction leaves the environmental state $|+\rangle$ unchanged on the system branch $|0\rangle$, while on the branch $|1\rangle$ it produces

$$
|e\rangle=\frac{(\cos\epsilon-\sin\epsilon)|0\rangle+(\cos\epsilon+\sin\epsilon)|1\rangle}{\sqrt2},
\qquad \langle e|+\rangle=\cos\epsilon.
$$

After interactions with $n$ distinct environment qubits, the joint state is

$$
|\Psi_n\rangle
=\alpha|0\rangle|+\rangle^{\otimes n}
+\beta|1\rangle|e\rangle^{\otimes n},
$$

and the [decoherence factor](../../../../../../decoherence-factor.md) is the product $(\cos\epsilon)^n$. Taking the [partial trace](../../../../../../partial-trace.md) gives

$$
\boxed{\rho_S^{(n)}=
\begin{pmatrix}
|\alpha|^2&\alpha\beta^*(\cos\epsilon)^n\\
\alpha^*\beta(\cos\epsilon)^n&|\beta|^2
\end{pmatrix}}.
$$

For small $\epsilon$, $(\cos\epsilon)^n\simeq e^{-n\epsilon^2/2}$: the populations remain fixed while the phase coherence decays. This is [environmental decoherence](../../../../../../quantum-decoherence.md), caused by entanglement with unobserved records rather than by a nonunitary evolution of the complete state.

A measurement in the computational basis cannot reveal the decay because its probabilities remain $|\alpha|^2$ and $|\beta|^2$. An interference measurement can. For example, measuring in the [Hadamard basis](../../../../../../hadamard-basis.md) gives

$$
P(\mathord\pm)=\frac12\left[1\pm2\operatorname{Re}(\alpha\beta^*)(\cos\epsilon)^n\right].
$$

Changing the measurement phase similarly accesses the imaginary part, so the shrinking interference visibility directly displays decoherence.

If the same environment qubit is reused, the conditional rotation accumulates coherently. After $n$ interactions the overlap is $\cos(n\epsilon)$ rather than $(\cos\epsilon)^n$, and the off-diagonal entries oscillate. Coherence vanishes at some times but returns periodically: this finite environment exhibits [quantum recoherence](../../../../../../quantum-recoherence.md) rather than effectively irreversible decay.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 325](../../../paper-325-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
