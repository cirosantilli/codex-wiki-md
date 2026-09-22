<h1 id="8/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Keep the actual odd-$n$ [GHZ state](../../../../../greenberger-horne-zeilinger-state.md) from the preceding calculation. Resolving its first [qubit](../../../../../qubit.md) in the [Hadamard basis](../../../../../hadamard-basis.md) gives

$$
|G\rangle=\frac{|+\rangle_1|\psi^-\rangle_{23}
+|-\rangle_1|\psi^+\rangle_{23}}{\sqrt2},\qquad
|\psi^\pm\rangle_{23}=\frac{|01\rangle\pm|10\rangle}{\sqrt2}.
$$

Thus the $+$ outcome leaves $|\psi^-\rangle_{23}$ and the $-$ outcome leaves $|\psi^+\rangle_{23}$, each with [probability](../../../../../probability.md) $1/2$. Conditional on a known result the remaining [qubits](../../../../../qubit.md) share a maximally [entangled state](../../../../../entangled-state.md).

When the result is not revealed, the appropriate [density matrix](../../../../../density-matrix-split.md) is the [probability](../../../../../probability.md)-weighted mixture from a [nonselective quantum measurement](../../../../../nonselective-quantum-measurement.md):

$$
\begin{aligned}
\rho_{23}
&=\frac12|\psi^-\rangle\langle\psi^-|+\frac12|\psi^+\rangle\langle\psi^+|\\
&=\frac12|01\rangle\langle01|+\frac12|10\rangle\langle10|\\
&=\frac12\bigl(|0\rangle\langle0|\otimes|1\rangle\langle1|\bigr)
+\frac12\bigl(|1\rangle\langle1|\otimes|0\rangle\langle0|\bigr)\\
&=\operatorname{diag}(0,1/2,1/2,0).
\end{aligned}
$$

The cross terms cancel. The displayed convex combination of [product states](../../../../../product-state.md) proves directly that this is a [separable quantum state](../../../../../separable-quantum-state.md). It still has perfect [computational-basis measurement](../../../../../quantum-measurement-in-the-computational-basis.md) anticorrelation, so it is not itself a [product state](../../../../../product-state.md). It also equals the [partial trace](../../../../../partial-trace.md) $\operatorname{Tr}_1|G\rangle\langle G|$, as required by the [no-communication theorem](../../../../../no-communication-theorem.md): a local [quantum measurement](../../../../../quantum-measurement-split.md) with an unobserved outcome cannot change the remote [reduced density matrix](../../../../../reduced-density-matrix.md).

## ↑ Ancestors (13)

1. [3](../3.md)
2. [8](../../8.md)
3. [7 and 8](../../../7-and-8-split.md)
4. [2005](../../../split.md)
5. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../../split.md)
6. [Laser science and quantum information processing course of the University of Oxford](../../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
7. [Year 4 of the physics course of the University of Oxford](../../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
