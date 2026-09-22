<h1 id="11/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [wave equation on a string](../../../../wave-equation-on-a-string.md) gives $c_j=\sqrt{T/\rho_j}$ and $\omega=c_jk_j$, hence

$$
\boxed{k_j=\omega\sqrt{\frac{\rho_j}{T}},\qquad T k_j^2=\rho_j\omega^2.}
$$

The tension is common across the join, and the frequency is unchanged by reflection and transmission at the stationary boundary.

Use the complex time convention $e^{i\omega t}$. The physical displacement is the real part of

$$
y_L=(Ae^{-ik_1x}+Be^{ik_1x})e^{i\omega t},\qquad
y_R=Ce^{-ik_2x}e^{i\omega t}.
$$

The first term is incident from the left, the second reflected to the left, and the right-side term transmitted to the right. Continuity of [displacement](../../../../displacement.md) gives $A+B=C$. At a massless join, continuity of the transverse [force](../../../../force-split.md) $T y_x$ gives $k_1(A-B)=k_2C$. Solving these two equations yields

$$
\boxed{r=\frac BA=\frac{k_1-k_2}{k_1+k_2},\qquad
 t=\frac CA=\frac{2k_1}{k_1+k_2}=1+r.}
$$

These are displacement-amplitude coefficients for [reflection at a density step on a string](../../../../reflection-at-a-density-step-on-a-string.md), not power fractions. Since the mean incident [power](../../../../power.md) is $T\omega k_1|A|^2/2$, the reflected and transmitted power fractions are $|r|^2$ and $(k_2/k_1)|t|^2$. They sum to one, as expected for the lossless join.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [11](../../11.md)
3. [2019 resit](../../../2019-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../c/solution.md)
