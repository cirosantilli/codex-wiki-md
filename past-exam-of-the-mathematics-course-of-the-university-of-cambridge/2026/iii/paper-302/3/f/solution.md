<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For the [trace trilinear form of a Lie algebra representation](../../../../../../trace-trilinear-form-of-a-lie-algebra-representation.md), the trace of a commutator vanishes:

$$
B([X,Y],Z,W)+B(Y,[X,Z],W)+B(Y,Z,[X,W])=0.
$$

Taking $X=T_b$, $Y=T_a$, $Z=T_c$, $W=T_d$ and expanding each [Lie bracket](../../../../../../lie-bracket.md) gives

$$
f^e{}_{ba}B_{cde}+f^e{}_{bc}B_{dae}+f^e{}_{bd}B_{ace}=0.
$$

Since $f_a{}^{bc}$ is antisymmetric in $b,c$,

$$
\begin{aligned}
f_a{}^{bc}B_{bcd}
&=\frac12f_a{}^{bc}\operatorname{Tr}([d(T_b),d(T_c)]d(T_d))\\
&=\frac12f_a{}^{bc}f_{bc}{}^eH(T_e,T_d).
\end{aligned}
$$

Raising indices with the inverse [Killing form](../../../../../../killing-form.md) gives $f_a{}^{bc}f_{bc}{}^e=\delta_a{}^e$ in the stated normalization. Using $H(T_e,T_d)=-\mu\delta_{ed}$ proves

$$
\boxed{f_a{}^{bc}B_{bcd}=-\frac\mu2\delta_{ad}.}
$$

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 302](../../../paper-302-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
