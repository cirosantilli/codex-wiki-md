<h1 id="section-a/a3/solution">Solution</h1>

↑ **Parent:** [A3](../a3.md)

After [field electron emission](../../../../field-electron-emission.md), let $h$ denote the plate separation of the [parallel-plate capacitor](../../../../parallel-plate-capacitor.md), which the question does not specify. The uniform capacitor [electric field](../../../../electric-field-split.md) has magnitude $E_c=|V|/h$, and a nonrelativistic [electron](../../../../electron.md) of [mass](../../../../mass.md) $m_e$ has constant [acceleration](../../../../acceleration.md) magnitude $a=eE_c/m_e$. The sign of its charge affects the direction of the radiation field but not its radiated [power](../../../../power.md).

In the supplied nonrelativistic [Liénard-Wiechert field](../../../../lienard-wiechert-field.md), $\dot{\boldsymbol\beta}=\mathbf a/c$. At polar angle $\theta$ to the [acceleration](../../../../acceleration.md), $|\widehat{\mathbf n}\times(\widehat{\mathbf n}\times\mathbf a)|=a\sin\theta$, hence

$$
E_{\rm rad}=\frac{ea\sin\theta}{4\pi\epsilon_0c^2R}.
$$

The outgoing [Poynting vector](../../../../poynting-vector.md) has magnitude $S=\epsilon_0cE_{\rm rad}^2$. Its radiated [power](../../../../power.md) per [solid angle](../../../../solid-angle.md) is therefore

$$
\frac{dP}{d\Omega}=R^2S=\frac{e^2a^2}{16\pi^2\epsilon_0c^3}\sin^2\theta.
$$

Using $\int\sin^2\theta\,d\Omega=8\pi/3$ gives the [Larmor formula](../../../../larmor-formula.md) and the requested constant [power](../../../../power.md) during the uniform-field part of the flight:

$$
\boxed{P=\frac{e^2a^2}{6\pi\epsilon_0c^3}
=\frac{e^4E_c^2}{6\pi\epsilon_0m_e^2c^3}
=\frac{e^4V^2}{6\pi\epsilon_0m_e^2c^3h^2}.}
$$

The brackets in the given field require the [acceleration](../../../../acceleration.md) at [retarded time](../../../../retarded-time.md); the radiation reaches the far observer after the propagation delay. This derivation assumes that [radiation reaction](../../../../radiation-reaction.md) is a small correction to the [acceleration](../../../../acceleration.md) and that the flight is nonrelativistic, for example $e|V|\ll m_ec^2$ for release from rest. Entry, emission and impact transients are not described by the uniform-field model. A result solely in terms of $V$ cannot be obtained without a plate spacing or a specified internal field.

## ↑ Ancestors (13)

1. [A3](../a3.md)
2. [Section A](../../section-a.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
5. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
