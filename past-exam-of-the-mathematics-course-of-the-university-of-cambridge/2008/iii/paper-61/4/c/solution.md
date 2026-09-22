<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $\gamma>0$ and zero initial cavity amplitude. Taking [Laplace transforms](../../../../../../laplace-transform.md) gives

$$
(s+\gamma/2)\widetilde a=-\sqrt\gamma\,\widetilde b_0,
\qquad \widetilde b_1=\sqrt\gamma\,\widetilde a+\widetilde b_0.
$$

Eliminating the mode yields the [passive cavity input-output transfer function](../../../../../../passive-cavity-input-output-transfer-function.md)

$$
\boxed{\widetilde b_1=G(s)\widetilde b_0,\qquad
G(s)=1-\frac\gamma{s+\gamma/2}=\frac{s-\gamma/2}{s+\gamma/2}.}
$$

Its unique pole is $s=-\gamma/2$, so the cavity's internal mode decays and its causal input-output response is stable. A nonzero initial amplitude would add $\sqrt\gamma\,a(0)/(s+\gamma/2)$ to the output, a decaying transient.

For a precise [Nyquist stability criterion](../../../../../../nyquist-stability-criterion.md) interpretation of this open cavity, rewrite the mode equation as an integrator with negative state feedback. Its return ratio is $L(s)=(\gamma/2)/s$, and its characteristic equation is $1+L(s)=0$. The frequency locus $L(i\omega)=-i\gamma/(2\omega)$ lies on the imaginary axis. The Nyquist indentation excluding the pole at the origin maps to a large semicircle in the right half-plane; the whole contour has no winding around $-1$. There are no right-half-plane open-loop poles within that indented contour, so there are no unstable characteristic zeros. There is also no zero-frequency characteristic root, since the physical characteristic polynomial is $s+\gamma/2$. This recovers asymptotic stability.

Do not use the plant $G$ as a return ratio without specifying an additional feedback connection. Indeed

$$
G(i\omega)=\frac{\omega^2-(\gamma/2)^2+i\gamma\omega}{\omega^2+(\gamma/2)^2},\qquad |G(i\omega)|=1,
$$

and its locus passes through $-1$ at $\omega=0$. That would indicate a marginal mode for a new unity-negative-feedback loop with characteristic factor $1+G$, but not instability of the original cavity. Part (e) supplies the actual return ratio $\alpha G$ for the beam-splitter network.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
