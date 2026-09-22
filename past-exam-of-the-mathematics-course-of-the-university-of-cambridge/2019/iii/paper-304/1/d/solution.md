<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Change variables in the defining integral from the fluctuation to the total field, $\varphi=\phi_0+\eta$. Then

$$
\begin{aligned}
e^{-W(J;\phi_0)/\hbar}
&=\int d\varphi\,
e^{-[S(\varphi)+J(\varphi-\phi_0)]/\hbar}\\
&=e^{J\phi_0/\hbar}e^{-W(J;0)/\hbar},
\end{aligned}
$$

and hence

$$
W(J;\phi_0)=W(J;0)-J\phi_0.
$$

It follows nonperturbatively that

$$
\chi=\partial_JW(J;\phi_0)
=\partial_JW(J;0)-\phi_0.
$$

Thus the same source $J_\chi$ corresponds at zero background to the mean field $\Phi=\chi+\phi_0$. Using the source-sign-compatible Legendre transform $\Gamma(\chi;\phi_0)=W(J_\chi;\phi_0)-J_\chi\chi$,

$$
\Gamma(\chi;\phi_0)
=W(J_\chi;0)-J_\chi(\chi+\phi_0)
=\Gamma(\chi+\phi_0;0).
$$

Renaming $\chi$ as $\eta$ gives the requested identity

$$
\boxed{\Gamma(\eta;\phi_0)=\Gamma(\phi_0+\eta;0).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
