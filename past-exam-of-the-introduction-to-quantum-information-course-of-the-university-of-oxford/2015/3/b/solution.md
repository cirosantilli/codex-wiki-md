<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $c=\langle e_0|e_1\rangle=ve^{i\alpha}$. The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) gives $0\leq v\leq1$ because the two environment states are normalized. Immediately after the interaction, the joint [quantum state](../../../../quantum-state.md) is

$$
|\Psi\rangle=\frac{|0\rangle|e_0\rangle+e^{i\varphi}|1\rangle|e_1\rangle}{\sqrt2}.
$$

Applying the last [Hadamard gate](../../../../hadamard-gate.md) gives

$$
|\Psi_{\rm out}\rangle=\frac12\left[
|0\rangle\bigl(|e_0\rangle+e^{i\varphi}|e_1\rangle\bigr)
+|1\rangle\bigl(|e_0\rangle-e^{i\varphi}|e_1\rangle\bigr)\right].
$$

Since the environment is unobserved, the [Born rule](../../../../born-rule.md) uses the squared [norm](../../../../norm.md) of the environment-valued coefficient of $|0\rangle$:

$$
P_0=\frac14\left[2+e^{i\varphi}\langle e_0|e_1\rangle
+e^{-i\varphi}\langle e_1|e_0\rangle\right].
$$

Thus the [Hadamard interference with environment overlap](../../../../hadamard-interference-with-environment-overlap.md) formula is

$$
\boxed{P_0(\varphi,v,\alpha)=\frac{1+v\cos(\varphi+\alpha)}2.}
$$

The plus sign follows from the explicitly chosen [phase gate](../../../../phase-gate.md) and the order $\langle e_0|e_1\rangle$ of the [inner product](../../../../inner-product-split.md). Equivalently, before the last [Hadamard gate](../../../../hadamard-gate.md) the [partial trace](../../../../partial-trace.md) over the environment gives

$$
\rho=\frac12\begin{pmatrix}
1&v e^{-i(\varphi+\alpha)}\\
v e^{i(\varphi+\alpha)}&1
\end{pmatrix}.
$$

The [complex environment overlap in qubit dephasing](../../../../complex-environment-overlap-in-qubit-dephasing.md) both reduces the [quantum coherence](../../../../quantum-coherence-in-a-specified-basis.md) by $v$ and adds a relative [quantum phase](../../../../quantum-phase.md) $\alpha$. Orthogonal environment states have $v=0$ and give $P_0=1/2$ for every $\varphi$. If $v=1$, the [quantum interference](../../../../quantum-interference.md) fringe has full contrast and is only shifted; the [qubit](../../../../qubit.md) has not become mixed. For $v=0$, $\alpha$ is immaterial.

Moving the interaction to between the first [Hadamard gate](../../../../hadamard-gate.md) and the [phase gate](../../../../phase-gate.md) gives

$$
\frac{|0\rangle|e_0\rangle+|1\rangle|e_1\rangle}{\sqrt2}
\xrightarrow{P_\varphi\otimes I}
\frac{|0\rangle|e_0\rangle+e^{i\varphi}|1\rangle|e_1\rangle}{\sqrt2},
$$

the identical joint [quantum state](../../../../quantum-state.md). Therefore **the expression is unchanged**. This is the [commutation of computational-basis dephasing and phase gates](../../../../commutation-of-computational-basis-dephasing-and-phase-gates.md); it uses the specified population-preserving interaction with the same environment states, rather than an arbitrary model of [quantum decoherence](../../../../quantum-decoherence.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
