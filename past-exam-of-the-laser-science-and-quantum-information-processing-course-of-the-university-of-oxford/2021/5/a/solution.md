<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the ordered polarization [basis](../../../../basis.md) $(|H\rangle,|V\rangle)$ and define the [Bell states](../../../../bell-state-split.md)

$$
|\Phi^\pm\rangle=\frac{|HH\rangle\pm|VV\rangle}{\sqrt2},\qquad
|\Psi^\pm\rangle=\frac{|HV\rangle\pm|VH\rangle}{\sqrt2}.
$$

Regrouping the four-[photon](../../../../photon.md) [quantum state](../../../../quantum-state.md) by channel pairs $(1,4)$ and $(2,3)$ gives

$$
\begin{aligned}
|\Phi^+\rangle_{12}|\Phi^+\rangle_{34}=\frac12\big(&|\Phi^+\rangle_{14}|\Phi^+\rangle_{23}
+|\Phi^-\rangle_{14}|\Phi^-\rangle_{23}\\
&+|\Psi^+\rangle_{14}|\Psi^+\rangle_{23}
+|\Psi^-\rangle_{14}|\Psi^-\rangle_{23}\big).
\end{aligned}
$$

For instance, projecting channels 2 and 3 on $\langle\Psi^-|$ retains the two original terms with inner polarizations $HV$ and $VH$, with opposite signs, leaving $(|HV\rangle-|VH\rangle)_{14}/(2\sqrt2)$. Its squared norm is $1/4$.

By the same [orthonormality](../../../../orthonormal-set.md) argument, each [Bell-basis measurement](../../../../bell-basis-measurement.md) outcome prepares the identically named [Bell state](../../../../bell-state-split.md) in channels 1 and 4, with

$$
\boxed{P(\Phi^+)=P(\Phi^-)=P(\Psi^+)=P(\Psi^-)=\frac14.}
$$

Before communication of the outcome, Alice and Bob's [density matrix](../../../../density-matrix-split.md) is $I_4/4$; the usable conditional [entanglement](../../../../entangled-state.md) is established by the announced [Bell-basis measurement](../../../../bell-basis-measurement.md) result. This assumes an ideal complete [Bell-basis measurement](../../../../bell-basis-measurement.md); ordinary passive linear optics alone does not deterministically distinguish all four polarization [Bell states](../../../../bell-state-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
