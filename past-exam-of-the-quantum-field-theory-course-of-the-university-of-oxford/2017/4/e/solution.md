<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Retain the specified leading poles and write $A=a_1/\epsilon$, $B=b_1/\epsilon^2$. Solving $g=g_0+Ag_0^2+Bg_0^3$ recursively gives

$$
g_0=g-Ag^2+(2A^2-B)g^3+O(g^4).
$$

The scale derivative must again be reexpressed in the [renormalized coupling](../../../../renormalized-coupling.md):

$$
\begin{aligned}
\beta(g)&=-\epsilon g_0\left(1+2Ag_0+3Bg_0^2\right)\\
&=-\epsilon g-\epsilon A g^2+2\epsilon(A^2-B)g^3+O(g^4)\\
&=\boxed{-\epsilon g-a_1g^2+\frac{2(a_1^2-b_1)}{\epsilon}g^3+O(g^4).}
\end{aligned}
$$

The [leading-pole consistency under coupling reparametrization](../../../../leading-pole-consistency-under-coupling-reparametrization.md) shows that a finite [renormalization-group beta function](../../../../beta-function-physics.md) requires the two-loop double-pole consistency condition

$$
\boxed{b_1=a_1^2.}
$$

The leading two-loop pole is fixed by the one-loop simple pole; it is not an independent parameter. This is an instance of the [simple-pole formulas for minimal-subtraction renormalization group functions](../../../../simple-pole-formulas-for-minimal-subtraction-renormalization-group-functions.md) and their higher-pole consistency relations.

The source's leading-pole truncation does **not** fix the finite two-loop coefficient of the [beta function](../../../../beta-function.md). For example, adding the omitted term $c_1g_0^3/\epsilon$ leaves the double-pole condition unchanged but contributes $-2c_1g^3$ to the finite [beta function](../../../../beta-function.md). Thus cancelling the displayed $1/\epsilon$ term is not a claim that the physical two-loop running vanishes.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
