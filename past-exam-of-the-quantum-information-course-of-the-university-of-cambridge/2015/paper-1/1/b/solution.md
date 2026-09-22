<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $c=\cos(\theta/2)$ and $s=\sin(\theta/2)$. The detector rotation is real and orthogonal, so its inverse is the same transformation. Substituting it gives

$$
|\Phi^C\rangle=\frac1{\sqrt2}\left[
(c|\uparrow\rangle+s|\downarrow\rangle)|d_\nearrow\rangle
+(s|\uparrow\rangle-c|\downarrow\rangle)|d_\swarrow\rangle\right].
$$

Thus the requested orthonormal system states are

$$
\boxed{|\nearrow\rangle=c|\uparrow\rangle+s|\downarrow\rangle,\qquad
|\swarrow\rangle=s|\uparrow\rangle-c|\downarrow\rangle.}
$$

The pure [density operator](../../../../../density-matrix-split.md) has not changed: this is only a different [Schmidt decomposition](../../../../../schmidt-decomposition.md) of a maximally entangled state. But choosing a nonselective [projective measurement](../../../../../projective-measurement.md) in this new detector basis gives a different operation and generally a different state:

$$
\boxed{\rho_\theta=\frac12\left(|\nearrow d_\nearrow\rangle\langle\nearrow d_\nearrow|
+|\swarrow d_\swarrow\rangle\langle\swarrow d_\swarrow|\right).}
$$

For an explicit matrix in the original ordered basis, write $q=c^2s^2$ and $h=cs(c^2-s^2)/2$. Then

$$
\rho_\theta=\begin{pmatrix}
\frac12-q&h&h&q\\h&q&q&-h\\h&q&q&-h\\q&-h&-h&\frac12-q
\end{pmatrix}.
$$

At $\theta=\pi/2$ the entries $(1,4)$ and $(2,3)$ are $1/4$, whereas they vanish in $\rho_{\rm up/down}$. Nevertheless, the system and detector individually each have [reduced density matrix](../../../../../reduced-density-matrix.md) $I/2$ for either mixture.

This is the [preferred-basis problem](../../../../../preferred-basis-problem.md): the correlated state alone does not specify which detector observable becomes a stable classical record. Arbitrarily declaring collapse in a Schmidt basis changes the physical prediction. The actual detector interaction and environment must supply the basis selection, rather than a mere choice of notation.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the quantum information course of the University of Cambridge](../../../../split.md)
6. [Quantum Information course of the University of Cambridge](../../../../../quantum-information-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
