<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the source action $S_{\rm src}=\int d^4x\,[J\phi+\bar\eta_\alpha\psi_\alpha+\bar\psi_\alpha\eta_\alpha]$, with independent [Grassmann variables](../../../../../grassmann-variable.md) used as sources $\eta,\bar\eta$ and left [functional derivatives](../../../../../functional-derivative.md). A scalar insertion is $(1/i)\delta/\delta J$. For the odd fields the ordered rules are

$$
\boxed{\phi\longleftrightarrow\frac1i\frac\delta{\delta J},\qquad
\bar\psi_\alpha\longleftrightarrow i\frac\delta{\delta\eta_\alpha},\qquad
\psi_\alpha\longleftrightarrow\frac1i\frac\delta{\delta\bar\eta_\alpha}.}
$$

The middle sign is not arbitrary: differentiating the rightmost odd source in $\bar\psi\eta$ from the left gives $\delta_L(\bar\psi\eta)/\delta\eta=-\bar\psi$. Derivative ordering must consequently match the displayed order of the fields; the rightmost derivative acts first.

Expand $\exp[ig\int\phi\bar\psi\psi]$ in its [power series](../../../../../power-series.md). Replace each field in every term by its source insertion, preserving the [fermion](../../../../../fermion.md) order. These derivatives can be pulled outside the free [path integral](../../../../../path-integral.md). Re-exponentiation gives the unnormalized [generating functional](../../../../../generating-functional.md)

$$
\boxed{Z[J,\bar\eta,\eta]=
\exp\left[ig\int d^4x
\left(\frac1i\frac\delta{\delta J(x)}\right)
\left(i\frac\delta{\delta\eta_\alpha(x)}\right)
\left(\frac1i\frac\delta{\delta\bar\eta_\alpha(x)}\right)\right]Z_0[J,\bar\eta,\eta].}
$$

Summation over the [spinor](../../../../../spinor.md) index is understood. Normalized [correlation functions](../../../../../correlation-function.md) require division by the same interacting $Z[0,0,0]$, which cancels [vacuum](../../../../../vacuum.md) factors; that division is separate from this operator identity.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
