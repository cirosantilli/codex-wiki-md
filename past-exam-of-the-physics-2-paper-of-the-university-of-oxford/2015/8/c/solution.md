<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep the source diagram's topology: the arm from the left supply node to $X$ contains $R_0$ and $C_0$ in series; the arm from $X$ to the right supply node is $C_1$; the arm from the left node to $Y$ is $R_1$; and the arm from $Y$ to the right node contains $R$ and $C$ in parallel. Their [complex impedances](../../../../electrical-impedance.md) are

$$
Z_0=R_0+\frac1{i\omega C_0},\qquad Z_1=\frac1{i\omega C_1},\qquad Z_p=\left(\frac1R+i\omega C\right)^{-1}.
$$

For this [capacitor bridge with series loss and a parallel standard arm](../../../../capacitor-bridge-with-series-loss-and-a-parallel-standard-arm.md), the detector carries no [electric current](../../../../electric-current.md) at balance. Taking the right supply node as zero [electric potential](../../../../electric-potential.md) and the left one as the source [voltage](../../../../voltage.md) $V_s$, the two [voltage dividers](../../../../voltage-divider.md) give $V_X=V_sZ_1/(Z_0+Z_1)$ and $V_Y=V_sZ_p/(R_1+Z_p)$. Equality of these complex [voltages](../../../../voltage.md) means equality at every time, rather than merely equality of their magnitudes. Cross multiplication yields $R_1Z_1=Z_0Z_p$. Thus

$$
R_0+\frac1{i\omega C_0}=R_1\frac{Z_1}{Z_p}=\frac{R_1C}{C_1}+\frac{R_1}{i\omega RC_1}.
$$

Equating real and imaginary parts gives

$$
\boxed{R_0=\frac{R_1C}{C_1},\qquad C_0=\frac{RC_1}{R_1}.}
$$

The two adjustable standards determine the two components of the unknown [complex impedance](../../../../electrical-impedance.md). Treating the lower-right arm as a series combination would give a different and incorrect balance equation for the source circuit. The result also gives the dimensionless [dielectric loss tangent](../../../../dielectric-loss-tangent.md) $\omega C_0R_0=\omega RC$ for the series-loss model.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
