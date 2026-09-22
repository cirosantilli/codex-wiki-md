<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\phi\in C_0^\infty(D)$, set

$$
f_\phi=-2\pi\Delta^{-1}\phi
=\int_DG_D(\mathord\cdot,y)\phi(y)\,dy
\in H_0^1(D)
$$

and define the distributional pairing by

$$
(h,\phi):=(h,f_\phi)_\nabla.
$$

It is centered Gaussian by the definition of the GFF. Integration by parts gives

$$
\begin{aligned}
\operatorname{Var}(h,\phi)
&=\|f_\phi\|_\nabla^2\\
&=\frac1{2\pi}\int_Df_\phi(-\Delta f_\phi)\,dx\\
&=\int_Df_\phi(x)\phi(x)\,dx\\
&=\iint_{D\times D}\phi(x)G_D(x,y)\phi(y)\,dx\,dy.
\end{aligned}
$$

This is the [Test-function pairing with a Gaussian free field](../../../../../../../test-function-pairing-with-a-gaussian-free-field.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 203](../../../../paper-203-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
