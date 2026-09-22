<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Each long wire lies in the other's [magnetic field](../../../../magnetic-field-split.md), $B=\mu_0I/(2\pi d)$. The magnetic [Lorentz force](../../../../lorentz-force.md) per unit length has magnitude

$$
\boxed{F'=\frac{\mu_0I^2}{2\pi d},\qquad\text{opposite currents repel}.}
$$

For the two-wire circuit's [self-inductance](../../../../self-inductance.md), a nonzero wire radius is essential. Introduce a radius $a_w\ll d$. Between the wires their [magnetic fields](../../../../magnetic-field-split.md) add. The external [magnetic flux linkage](../../../../magnetic-flux-linkage.md) per unit length through the connecting ribbon is, to leading order in $a_w/d$,

$$
\Phi'=\int_{a_w}^{d-a_w}\frac{\mu_0I}{2\pi}\left(\frac1x+\frac1{d-x}\right)dx
=\frac{\mu_0I}{\pi}\ln\frac{d-a_w}{a_w}.
$$

It follows that the leading thin-wire loop [self-inductance](../../../../self-inductance.md) per unit length is

$$
\boxed{L'_{\rm ext}\simeq\frac{\mu_0}{\pi}\ln\frac d{a_w}.}
$$

It is the loop value for the pair, not the contribution of just one conductor. Corrections from the wire interior depend on the current distribution: for nonmagnetic round wires with uniform direct [electric current](../../../../electric-current.md), the pair contributes another $\mu_0/(4\pi)$; for a surface current the internal contribution is zero. The leading logarithm is common to both models.

**TODO (source data):** the source gives no wire radius or current-distribution convention. There is no finite radius-independent value of the requested [self-inductance](../../../../self-inductance.md): taking ideal zero-width wires sends $L'_{\rm ext}$ to infinity. The [force](../../../../force-split.md) and the parameterized leading [self-inductance](../../../../self-inductance.md) above are determined, but a unique finite answer requires that additional specification. For example, changing $a_w$ to $a_w/2$ changes the leading result by $\mu_0\ln2/\pi$ even at fixed separation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
