<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First derive the contracted [gamma matrices](../../../../../gamma-matrices.md) identities from the [Clifford algebra](../../../../../clifford-algebra.md) in four dimensions. Moving the outer [gamma matrix](../../../../../gamma-matrices.md) through two factors gives

$$
\gamma_\rho\gamma_\alpha\gamma_\beta\gamma^\rho=4g_{\alpha\beta}\mathbf1.
$$

Moving it through three factors, and using this two-factor result, gives

$$
\begin{aligned}
\gamma_\rho\gamma_\alpha\gamma_\beta\gamma_\gamma\gamma^\rho
&=2\gamma_\beta\gamma_\gamma\gamma_\alpha-4g_{\beta\gamma}\gamma_\alpha\\
&=-2\gamma_\gamma\gamma_\beta\gamma_\alpha.
\end{aligned}
$$

Consequently $\gamma^\nu\not b\gamma_\mu\not c\gamma_\nu=-2\not c\gamma_\mu\not b$ and $\gamma_\mu\not b\not d\gamma^\mu=4(b\cdot d)\mathbf1$. Apply these in succession:

$$
\begin{aligned}
T&=\operatorname{tr}(\not a\gamma^\nu\not b\gamma_\mu\not c\gamma_\nu\not d\gamma^\mu)\\
&=-2\operatorname{tr}(\not a\not c\gamma_\mu\not b\not d\gamma^\mu)\\
&=-8(b\cdot d)\operatorname{tr}(\not a\not c)
=\boxed{-32(a\cdot c)(b\cdot d)}.
\end{aligned}
$$

The final step uses $\operatorname{tr}(\gamma^\alpha\gamma^\beta)=4g^{\alpha\beta}$. This is a genuinely four-dimensional instance of the [gamma matrix trace identities](../../../../../gamma-matrix-trace-identities.md); using it unchanged inside a $D$-dimensional loop calculation would require separate justification.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
