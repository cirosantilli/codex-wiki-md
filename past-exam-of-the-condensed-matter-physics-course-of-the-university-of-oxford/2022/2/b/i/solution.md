<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a long chain of length $L$ with periodic boundary conditions, each [spin](../../../../../spin.md) has $L\,dk/(2\pi)$ [quantum states](../../../../../quantum-state.md) in a [wavenumber](../../../../../wavenumber.md) interval $dk$. Including two [spin](../../../../../spin.md) states, a full [energy band](../../../../../energy-band.md) contains $2L/a$ [electrons](../../../../../electron.md). The [state counting in a Bloch band](../../../../../state-counting-in-a-bloch-band.md) therefore gives the [energy density](../../../../../energy-density.md)

$$
\mathcal U(\epsilon)=\frac1\pi\int_{\text{one zone}}E_-(k)\,dk
=\frac{E_{\rm ZB}}a\int_{-1}^1
\left[1+y^2-\sqrt{4y^2+\epsilon^2}\right]dy.
$$

The integral of $1+y^2$ is $8/3$. For $\epsilon>0$, the even square-root integral is

$$
\int_{-1}^1\sqrt{4y^2+\epsilon^2}\,dy
=\sqrt{4+\epsilon^2}+\frac{\epsilon^2}{2}
\ln\frac{2+\sqrt{4+\epsilon^2}}{\epsilon}.
$$

For example, this follows by setting $u=2y$, applying the supplied antiderivative, and evaluating both endpoints; the lower-end [logarithm](../../../../../logarithm.md) contributes $\ln\epsilon$. Hence

$$
\boxed{\mathcal U(\epsilon)=\frac{E_{\rm ZB}}a
\left[\frac83-\sqrt{4+\epsilon^2}
-\frac{\epsilon^2}{2}\ln\frac{2+\sqrt{4+\epsilon^2}}{\epsilon}\right].}
$$

The continuous zero-coupling limit is $\mathcal U(0)=2E_{\rm ZB}/(3a)$. This agrees with directly integrating the one-dimensional [free electron model](../../../../../free-electron-model.md) up to $k_F=\pi/a$ at two [electrons](../../../../../electron.md) per [unit cell](../../../../../unit-cell.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the condensed matter physics course of the University of Oxford](../../../../split.md)
6. [Condensed matter physics course of the University of Oxford](../../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
7. [Year 3 of the physics course of the University of Oxford](../../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
