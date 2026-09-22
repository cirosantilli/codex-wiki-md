<h1 id="11/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep the $e^{i\omega t}$ convention of [solution](../b/solution.md). The point mass has the common displacement $y(0,t)=Ce^{i\omega t}$, so $A+B=C$ still holds. Its net transverse [force](../../../../force-split.md) is the right-side string force minus the left-side one:

$$
-M\omega^2C=T\big[-ik_2C-(-ik_1A+ik_1B)\big].
$$

After rearranging,

$$
k_1T(A-B)=(k_2T+iM\omega^2)C.
$$

Eliminate $C=A+B$ to obtain the [reflection at a string junction carrying a point mass](../../../../reflection-at-a-string-junction-carrying-a-point-mass.md):

$$
\boxed{r=\frac{(k_1-k_2)T-iM\omega^2}{(k_1+k_2)T+iM\omega^2},\qquad
 t=\frac{2k_1T}{(k_1+k_2)T+iM\omega^2}.}
$$

Continuity checks the identity $t=1+r$. Setting $M=0$ recovers [solution](../b/solution.md), while $M\to\infty$ at fixed nonzero frequency gives $r\to-1$ and $t\to0$, the fixed-boundary limit.

The signs of the imaginary terms depend on the time convention. With $e^{-i\omega t}$ and conjugate spatial conventions, both coefficients are complex conjugated; the source's displayed signs agree with the convention used here.

There is no damping in the point mass, so its cycle-averaged absorbed [power](../../../../power.md) is zero. Writing $D=T^2(k_1+k_2)^2+M^2\omega^4$, the power fractions are

$$
\mathcal R=\frac{T^2(k_1-k_2)^2+M^2\omega^4}{D},\qquad
\mathcal T=\frac{4T^2k_1k_2}{D},\qquad\mathcal R+\mathcal T=1.
$$

This provides an independent conservation check on both the numerator signs and the transmission prefactor.

## ↑ Ancestors (12)

1. [C](../c.md)
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
