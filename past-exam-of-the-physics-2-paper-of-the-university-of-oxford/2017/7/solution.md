<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The original circuit has $R_1$ and $C$ in series between the input and the inverting node, with $R_2$ providing feedback and the noninverting node grounded. An ideal [operational amplifier](../../../operational-amplifier.md) in stable linear [negative feedback](../../../negative-feedback.md) draws no input [electric current](../../../electric-current.md) and holds the inverting node at [virtual ground](../../../virtual-ground.md). For [phasors](../../../phasor.md) proportional to $e^{i\omega t}$, the input [complex impedance](../../../electrical-impedance.md) is $Z_1=R_1+1/(i\omega C)$. [Kirchhoff's current law](../../../kirchhoff-node-law.md) gives $\widetilde V_{\rm in}/Z_1=-\widetilde V_{\rm out}/R_2$, hence

$$
\boxed{H(\omega)=\frac{\widetilde V_{\rm out}}{\widetilde V_{\rm in}}
=-\frac{i\omega R_2C}{1+i\omega R_1C},\qquad
|H|=\frac{\omega R_2C}{\sqrt{1+\omega^2R_1^2C^2}}.}
$$

This is an inverting [high-pass filter](../../../high-pass-filter.md). Its [phase](../../../phase-waves.md) can be chosen continuously as

$$
\boxed{\arg H=-\frac\pi2-\tan^{-1}(\omega R_1C).}
$$

Thus $V_{\rm out}(t)=V_0|H|\cos(\omega t+\arg H)$. The ratio above is a [phasor](../../../phasor.md) ratio, not an instantaneous ratio at input zero crossings. Setting $R_1=R_2$ does not remove the [capacitor](../../../capacitor.md)'s [phase](../../../phase-waves.md): the output lags by $90^\circ+\tan^{-1}(\omega R_1C)$, between $90^\circ$ and $180^\circ$. At $\omega R_1C=1$ the lag is $135^\circ$; only for $\omega R_1C\gg1$ does it approach $180^\circ$. Being within the amplifier's own [bandwidth](../../../bandwidth-signal-processing.md) does not specify the external RC corner [frequency](../../../frequency.md).

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2017](../../2017-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
