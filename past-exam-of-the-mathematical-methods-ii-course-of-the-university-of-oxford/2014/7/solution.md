<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Apply the product-to-sum identity directly to the stated modulation:

$$
\boxed{A=a\cos(\omega t-kx)+\frac b2\cos[(\omega+\omega_m)t-kx]+\frac b2\cos[(\omega-\omega_m)t-kx].}
$$

The carrier has angular frequency $\omega$ and the two [modulation sidebands](../../../modulation-sideband.md) have angular frequencies $\omega\pm\omega_m$, each with amplitude $b/2$.

**Propagation qualification.** In the literal formula, all three terms have the same spatial wavenumber. That identity is correct, but a time-only amplitude applied everywhere is not generally a freely propagating wave at speed $c$. For $k=\omega/c$, applying $\partial_t^2-c^2\partial_x^2$ to the stated field gives $A_0''\cos(\omega t-kx)-2\omega A_0'\sin(\omega t-kx)$, which at $x=t=0$ equals $-b\omega_m^2\ne0$ when the modulation is nontrivial.

A physical modulation launched at a boundary and travelling without dispersion has envelope $a+b\cos[\omega_m(t-x/c)]$. The same expansion then has sideband wavenumbers $k_\pm=(\omega\pm\omega_m)/c$, while its value at $x=0$ agrees with the given time-modulated signal. This distinguishes the requested frequency decomposition from an unsupported fixed-wavenumber propagation claim.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2014](../../2014-split.md)
3. [Past exam of the mathematical methods II course of the University of Oxford](../../split.md)
4. [Mathematical methods II course of the University of Oxford](../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
