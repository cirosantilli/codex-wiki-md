<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $\{\gamma^a,\gamma^b\}=2\eta^{ab}$ and $\gamma^{ab}=\gamma^{[a}\gamma^{b]}=[\gamma^a,\gamma^b]/2$, with unit-weight antisymmetrization. The [Clifford algebra](../../../../../clifford-algebra.md) first gives

$$
\gamma_a\gamma^m\gamma^a=(2-D)\gamma^m,\qquad
\gamma_a\gamma_b\gamma^a=(2-D)\gamma_b.
$$

Expand the two antisymmetrized [gamma matrices](../../../../../gamma-matrices.md) using $\gamma_{ab}=\gamma_a\gamma_b-\eta_{ab}$:

$$
\gamma_{ab}\gamma^m\gamma^{ab}
=\gamma_a\gamma_b\gamma^m\gamma^a\gamma^b-D\gamma^m.
$$

Anticommuting $\gamma^m$ past the next contracted factor gives

$$
\begin{aligned}
\gamma_a\gamma_b\gamma^m\gamma^a\gamma^b
&=-\gamma_a\gamma_b\gamma^a\gamma^m\gamma^b+2\gamma^m\gamma_b\gamma^b\\
&=-(2-D)\gamma_b\gamma^m\gamma^b+2D\gamma^m\\
&=\bigl[2D-(D-2)^2\bigr]\gamma^m.
\end{aligned}
$$

Subtracting the remaining $D\gamma^m$ gives the [gamma-matrix vector sandwich](../../../../../gamma-matrix-vector-sandwich.md)

$$
\boxed{\alpha=-(D-1)(D-4).}
$$

In particular it vanishes in four dimensions. The result is independent of the choice of Lorentz signature when all indices are contracted consistently. Defining the bivector without its factor $1/2$ would multiply $\alpha$ by four.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [Section A](../section-a.md)
3. [Paper 53](../../paper-53-split.md)
4. [Iii](../../split.md)
5. [2003](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
