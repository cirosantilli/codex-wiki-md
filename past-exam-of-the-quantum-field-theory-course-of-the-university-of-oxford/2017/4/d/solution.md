<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At fixed regulator abbreviate

$$
A(\epsilon)=\frac{a_1}{\epsilon}+a_2+a_3\epsilon+\cdots,\qquad
C(\epsilon)=\frac{z_1}{\epsilon}+z_2+z_3\epsilon+\cdots.
$$

The [coupling](../../../../coupling.md) expansion is $g=g_0+Ag_0^2+O(g_0^3)$, whose inverse is $g_0=g-Ag^2+O(g^3)$. Using part c before removing the regulator,

$$
\begin{aligned}
\beta(g)&=-\epsilon g_0(1+2Ag_0)+O(g_0^3)\\
&=-\epsilon g-\epsilon A g^2+O(g^3),\\
\gamma(g)&=-\epsilon g_0\frac{C}{1+Cg_0}+O(g_0^2)
=-\epsilon Cg+O(g^2).
\end{aligned}
$$

Therefore the regulator-free coefficients at the orders determined by the supplied expansions are

$$
\boxed{\beta(g)=-a_1g^2+O(g^3),\qquad\gamma(g)=-z_1g+O(g^2).}
$$

The canonical term $-\epsilon g$ vanishes, and the factors of $\epsilon$ cancel the simple poles. The finite coefficients $a_2,z_2$ and higher positive powers of $\epsilon$ do not enter these leading regulator-free terms. Inverting the [coupling](../../../../coupling.md) is essential: substituting $g_0=g$ too early would incorrectly give $-2a_1g^2$.

The calculation establishes finiteness only at the displayed perturbative orders. Higher-order pole cancellations require the higher-order coefficients, as the next part makes explicit.

## ↑ Ancestors (12)

1. [D](../d.md)
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
