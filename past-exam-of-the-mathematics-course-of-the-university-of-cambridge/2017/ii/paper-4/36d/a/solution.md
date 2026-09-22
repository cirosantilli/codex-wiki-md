<h1 id="36d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $G=c=1$ and the physical [real part](../../../../../../real-part.md) of the printed [plane wave](../../../../../../plane-wave.md). Its null wavevector obeys $k^\alpha k_\alpha=0$, so each component satisfies $\Box h_{\alpha\beta}=0$. Direct differentiation of the defined stress tensor gives

$$
\partial^\nu\tau_{\mu\nu}=\frac1{32\pi}(\partial^\nu\partial_\mu h^{\alpha\beta})(\partial_\nu h_{\alpha\beta})
+\frac1{32\pi}(\partial_\mu h^{\alpha\beta})\Box h_{\alpha\beta}
=\frac12\partial_\mu\tau^\nu{}_\nu.
$$

The [trace](../../../../../../matrix-trace.md) is proportional to $k^\nu k_\nu$ for a single [plane wave](../../../../../../plane-wave.md) and hence vanishes. Therefore

$$
\boxed{\tau^\nu{}_\nu=0,\qquad\partial^\nu\tau_{\mu\nu}=0.}
$$

This is local [conservation of energy](../../../../../../conservation-of-energy.md) and [momentum conservation](../../../../../../momentum-conservation.md); spatial integration gives conserved total charges when the boundary flux vanishes. For a finite-amplitude complex phasor, one takes the real field before quadratic products and may time-average: $\langle\tau_{\mu\nu}\rangle=k_\mu k_\nu H^{\alpha\beta}\overline{H}_{\alpha\beta}/(64\pi)$ in [transverse-traceless gauge](../../../../../../transverse-traceless-gauge.md). Its [energy density](../../../../../../energy-density.md) is nonnegative and its flux travels in the positive $z$ direction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [36D](../../36d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
