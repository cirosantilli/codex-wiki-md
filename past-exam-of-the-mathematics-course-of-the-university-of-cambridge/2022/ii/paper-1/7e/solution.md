<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Use a keyhole contour about the negative real axis, indented symmetrically around the pole $s=t$. The jump of $s^{z-1}$ across the cut is determined by the chosen branch, and the small and large circular contributions vanish for $0<\operatorname{Re}z<1$. The [residue theorem](../../../../../residue-theorem.md), with the symmetric indentation interpreted as a [Cauchy principal value](../../../../../cauchy-principal-value.md), gives

$$
\boxed{\operatorname{PV}\int_{-\infty}^{\infty}
\frac{s^{z-1}}{s-t}\,ds=\pi i\,t^{z-1}}.
$$

Splitting the real axis at zero and substituting $s\mapsto-s$ in the negative part gives two linear relations. Solving them yields, for real $0<z<1$,

$$
\boxed{\int_0^\infty\frac{s^{z-1}}{s+t}\,ds
=\pi t^{z-1}\csc(\pi z)},
$$



$$
\boxed{\operatorname{PV}\int_0^\infty\frac{s^{z-1}}{s-t}\,ds
=-\pi t^{z-1}\cot(\pi z)}.
$$

Both sides are holomorphic functions of $z$ throughout the vertical strip $0<\operatorname{Re}z<1$: convergence is locally uniform there, and the trigonometric expressions are holomorphic away from integer poles. The [identity theorem](../../../../../identity-theorem.md) therefore extends the identities from real $z$ to the whole strip.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
