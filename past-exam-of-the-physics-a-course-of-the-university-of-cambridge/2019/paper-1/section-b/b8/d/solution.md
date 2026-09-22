<h1 id="section-b/b8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [boundary force in an infinite square well](../../../../../../boundary-force-in-an-infinite-square-well.md) is obtained from the kinetic [momentum](../../../../../../momentum-split.md) flux at each wall. With $C_1=\hbar^2\pi^2/(2mL^3)=E_1/L$, the derivatives of the state in part (c) are

$$
\Psi'(0,t)=\frac{\pi}{L^{3/2}}(e^{-iE_1t/\hbar}+2e^{-iE_2t/\hbar}),\quad \Psi'(L,t)=\frac{\pi}{L^{3/2}}(-e^{-iE_1t/\hbar}+2e^{-iE_2t/\hbar}).
$$

The outward force magnitudes are $P_j=(\hbar^2/2m)|\Psi'(x_j,t)|^2$. Taking positive force to mean rightwards, the forces exerted by the particle on the walls are

$$
\boxed{F_{\mathrm{left}}=-C_1(5+4\cos\Omega t),\qquad F_{\mathrm{right}}=C_1(5-4\cos\Omega t).}
$$

Both point outwards at all times, but their magnitudes oscillate out of phase. This force formula follows directly by differentiating the mean particle [momentum](../../../../../../momentum-split.md) and integrating the interior [Schrödinger equation](../../../../../../schrodinger-equation.md) by parts: $d\langle p\rangle/dt=(\hbar^2/2m)(|\Psi'(0)|^2-|\Psi'(L)|^2)$. As a check, the net force on the particle is $8C_1\cos\Omega t=m\,d^2\langle x\rangle/dt^2$, the opposite of the net force on the two walls.

A classical particle of [energy](../../../../../../energy-split.md) $E=\langle E\rangle$ transfers [momentum](../../../../../../momentum-split.md) $2mv$ in each collision with a particular wall, and returns to that wall after $2L/v$. Its mean outward force on that wall is

$$
\boxed{\overline P_{\mathrm{classical}}=\frac{2mv}{2L/v}=\frac{2E}{L}=5C_1=\overline P_{\mathrm{quantum}}.}
$$

Thus the time averages agree separately at each wall, although the classical force consists of collision impulses and the quantum expectation varies continuously. Constant mean [energy](../../../../../../energy-split.md) alone does not make the instantaneous quantum wall forces constant; their unequal instantaneous values supply the oscillation of $\langle x\rangle$.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
