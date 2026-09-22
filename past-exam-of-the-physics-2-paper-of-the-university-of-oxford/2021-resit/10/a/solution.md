<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a circular [current loop](../../../../current-loop.md), the [Biot-Savart law](../../../../biot-savart-law.md) is

$$
d\mathbf B=\frac{\mu_0I}{4\pi}\frac{d\boldsymbol\ell\times\mathbf s}{s^3},
$$

where $\mathbf s$ points from a [current element](../../../../current-element.md) to the field point. Choose the loop in the $yz$ plane, with observation point $x\widehat{\mathbf x}$. A parametrization consistent with positive axial [magnetic field](../../../../magnetic-field-split.md) is

$$
\mathbf r'(\varphi)=(0,a\cos\varphi,a\sin\varphi),\quad
d\boldsymbol\ell=(0,-a\sin\varphi,a\cos\varphi)d\varphi,\quad
\mathbf s=(x,-a\cos\varphi,-a\sin\varphi).
$$

Then $s=\sqrt{a^2+x^2}$ and

$$
d\boldsymbol\ell\times\mathbf s
=(a^2,ax\cos\varphi,ax\sin\varphi)d\varphi.
$$

The transverse contributions cancel around the [circle](../../../../circle.md), leaving the [on-axis magnetic field of a circular current loop](../../../../on-axis-magnetic-field-of-a-circular-current-loop.md)

$$
\boxed{\mathbf B(x)=\frac{\mu_0Ia^2}{2(a^2+x^2)^{3/2}}\widehat{\mathbf x}.}
$$

The [right-hand rule](../../../../right-hand-rule.md) fixes its direction; reversing the [electric current](../../../../electric-current.md) reverses the [magnetic field](../../../../magnetic-field-split.md). At the centre this becomes $\mu_0I/(2a)$, and far away it decays as $|x|^{-3}$, as expected for a [magnetic dipole](../../../../magnetic-dipole.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
