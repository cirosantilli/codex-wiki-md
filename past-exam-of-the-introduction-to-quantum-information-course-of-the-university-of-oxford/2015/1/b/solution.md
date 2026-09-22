<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\oplus$ for bitwise [exclusive or](../../../../exclusive-or.md). Both [quantum registers](../../../../quantum-register.md) begin in $|0^n\rangle$. After the first [Hadamard transform](../../../../hadamard-transform.md) their joint [quantum state](../../../../quantum-state.md) is

$$
2^{-n/2}\sum_{x\in\{0,1\}^n}|x\rangle|0^n\rangle.
$$

The [quantum oracle](../../../../quantum-oracle.md) $U_f$ maps each component $|x\rangle|0^n\rangle$ to $|x\rangle|f(x)\rangle$. By [linearity](../../../../linearity.md), the required [quantum state](../../../../quantum-state.md) is therefore

$$
\boxed{|\Psi\rangle=2^{-n/2}\sum_{x\in\{0,1\}^n}|x\rangle|f(x)\rangle.}
$$

The different first-register [computational-basis states](../../../../computational-basis-state.md) are [orthogonal](../../../../orthogonal-vectors.md), so there are $2^n$ orthogonal joint components of squared [probability amplitude](../../../../probability-amplitude.md) $2^{-n}$, even though some second-register values coincide. Thus the displayed [quantum state](../../../../quantum-state.md) is normalized.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
