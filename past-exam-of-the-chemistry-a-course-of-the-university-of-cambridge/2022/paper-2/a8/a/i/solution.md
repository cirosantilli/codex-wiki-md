<h1 id="a8/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume a dilute classical [ideal gas](../../../../../../ideal-gas-split.md) of $N$ indistinguishable, noninteracting particles, with translational states dense enough to replace their sum by a continuum integral. Separate translation from all internal degrees of freedom. Then

$$
Q_{\rm trans}=\frac{q_{\rm trans}^{\,N}}{N!},\qquad
q_{\rm trans}=\frac V{\Lambda^3},\qquad
\Lambda=\frac h{\sqrt{2\pi mk_{\rm B}T}}.
$$

Using [Stirling's approximation](../../../../../../stirling-formula.md) in the [Helmholtz free energy](../../../../../../helmholtz-free-energy.md),

$$
A_{\rm trans}=-Nk_{\rm B}T\left[\ln\frac{V}{N\Lambda^3}+1\right].
$$

Differentiate at fixed $N,V$. Since $\Lambda^{-3}\propto T^{3/2}$,

$$
S_{\rm trans}=-\left(\frac{\partial A_{\rm trans}}{\partial T}\right)_{N,V}
=Nk_{\rm B}\left[\ln\frac{V}{N\Lambda^3}+\frac52\right].
$$

Only after this derivative set $N=N_A$ and $V=RT/p^\circ$ for one mole at [standard pressure](../../../../../../standard-pressure.md):

$$
\boxed{\frac{S^\circ_{\rm trans,m}}R
=\ln\left[\left(\frac{2\pi mk_{\rm B}T}{h^2}\right)^{3/2}\frac{RT}{p^\circ}\right]
-\ln N_A+\frac52.}
$$

This is the translational [Sackur-Tetrode equation](../../../../../../sackur-tetrode-equation.md). The $N!$ factor is essential for the correct extensive [entropy](../../../../../../entropy-split.md); replacing $V$ by a temperature-dependent standard molar volume before taking the fixed-volume derivative would give the wrong constant term.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [A8](../../../a8.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the chemistry A course of the University of Cambridge](../../../../../split.md)
7. [Chemistry A course of the University of Cambridge](../../../../../../chemistry-a-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
