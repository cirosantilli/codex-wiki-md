<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $k_D=k_r+k_{nr}$, so the lifetime without transfer is $\tau_D=1/k_D$. For a fixed isolated donor–acceptor pair, the specified transfer rate is $k_T=k_D(R_0/R)^6$. Inserting this rate into the definition of [FRET efficiency](../../../../fret-efficiency.md) gives

$$
E=\frac{k_D(R_0/R)^6}{k_D[1+(R_0/R)^6]}
=\boxed{\frac1{1+(R/R_0)^6}}.
$$

The donor population in the presence of the acceptor obeys $\dot N_D=-(k_D+k_T)N_D$, so its [fluorescence](../../../../fluorescence-split.md) decays exponentially with lifetime $\tau_{DA}=1/(k_D+k_T)$. Therefore

$$
\frac{\tau_{DA}}{\tau_D}=\frac{k_D}{k_D+k_T}=1-E,
\qquad\boxed{E=1-\frac{\tau_{DA}}{\tau_D}.}
$$

Both relations assume the donor's nontransfer rates are unchanged by adding the acceptor, a single approximately fixed separation during each excited-state lifetime, and an available acceptor. The transfer law also presumes the usual weak-coupling dipole approximation and the spectral and orientation conditions contained in $R_0$. If the reference donor is differently quenched, the lifetime difference cannot all be attributed to transfer. Heterogeneous mixtures or a fluctuating separation can produce multiexponential decay, in which case blindly substituting an arbitrary fitted average lifetime into the single-pair formula need not give the ensemble's mean efficiency.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
