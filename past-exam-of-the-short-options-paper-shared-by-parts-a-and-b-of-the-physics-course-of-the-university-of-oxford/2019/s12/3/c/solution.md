<h1 id="s12/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The observed $90^\circ+30^\circ$ substeps sum to $120^\circ$, consistent with three catalytic cycles per revolution of $F_1$-[ATPase](../../../../../atpase.md). Surface attachment fixes the $\beta$-subunit frame while the gold-labelled $\gamma$ shaft reports relative rotation. A finite dwell before the smaller step indicates hidden chemical transitions rather than a completely smooth motor.

Suppose two irreversible independent first-order transitions, with rates $k_a$ and $k_b$, must occur sequentially before the $30^\circ$ step. Their waiting times $X_a$ and $X_b$ have [exponential distributions](../../../../../exponential-distribution.md), and $\tau=X_a+X_b$. [Convolution](../../../../../convolution.md) gives

$$
P(\tau)=\int_0^\tau k_ae^{-k_at}k_be^{-k_b(\tau-t)}dt
=\boxed{\frac{k_ak_b}{k_a-k_b}(e^{-k_b\tau}-e^{-k_a\tau})},\qquad\tau\ge0.
$$

This [probability density](../../../../../probability-density.md) integrates to one and has $\langle\tau\rangle=k_a^{-1}+k_b^{-1}$. For equal rates its continuous limit is $P(\tau)=k^2\tau e^{-k\tau}$, not a singular distribution. In particular $P(0)=0$ distinguishes two resolved sequential waits from a single exponential wait. Hydrolysis and product release are plausible underlying chemical events, but the waiting-time fit alone neither assigns their order nor uniquely identifies which biochemical event causes each substep. Concentration dependence or independent labelling would be needed for that assignment.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [S12](../../../s12.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
