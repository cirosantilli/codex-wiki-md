<h1 id="9a/solution">Solution</h1>

↑ **Parent:** [9A](../9a.md)

The [equation of motion in a rotating frame](../../../../../equation-of-motion-in-a-rotating-frame.md) with constant [angular velocity](../../../../../angular-velocity.md) $\boldsymbol\omega$ is

$$
m\left[\ddot{\mathbf x}+2\boldsymbol\omega\times\dot{\mathbf x}
+\boldsymbol\omega\times(\boldsymbol\omega\times\mathbf x)\right]=\mathbf F.
$$

With $\mathbf F=-4m\omega^2\mathbf x$ and $\boldsymbol\omega=(0,0,\omega)$, this becomes

$$
\ddot x-2\omega\dot y+3\omega^2x=0,\qquad
\ddot y+2\omega\dot x+3\omega^2y=0,\qquad
\ddot z+4\omega^2z=0.
$$

The given initial data make $z=0$. For the [complex coordinate](../../../../../complex-coordinate.md) $\zeta=x+iy$, the planar equations combine into

$$
\ddot\zeta+2i\omega\dot\zeta+3\omega^2\zeta=0.
$$

Its [characteristic roots](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md) are $i\omega$ and $-3i\omega$. Applying $\zeta(0)=1$, $\dot\zeta(0)=0$ gives $\zeta=\tfrac34e^{i\omega t}+\tfrac14e^{-3i\omega t}$. The triple-angle identities reduce this [astroid motion of a harmonic oscillator in a rotating frame](../../../../../astroid-motion-of-a-harmonic-oscillator-in-a-rotating-frame.md) to

$$
\boxed{(x,y,z)=(\cos^3\omega t,\sin^3\omega t,0).}
$$

It traces an [astroid](../../../../../astroid.md). Differentiating gives the relative [speed](../../../../../speed.md)

$$
|\dot{\mathbf x}|^2
=9\omega^2\sin^2\omega t\cos^2\omega t
=\frac94\omega^2\sin^2(2\omega t).
$$

For $\omega>0$, its maxima occur at $t=(2n+1)\pi/(4\omega)$, with

$$
\boxed{|\dot{\mathbf x}|_{\max}=\frac{3\omega}{2}.}
$$

This is speed measured in the specified [rotating frame](../../../../../rotating-reference-frame.md). The same physical motion has inertial complex coordinate $e^{i\omega t}\zeta=\cos(2\omega t)+(i/2)\sin(2\omega t)$, an [ellipse](../../../../../ellipse.md); its initial [velocity](../../../../../velocity.md) is the frame-rotation contribution even though the initial relative [velocity](../../../../../velocity.md) is zero.

<a id="9a/image-the-oscillator-s-astroid-in-rotating-coordinates-ellipse-in-inertial-coordinates-and-maxima-of-relative-speed"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-4-rotating-oscillator.png)

**[Figure 1](#9a/image-the-oscillator-s-astroid-in-rotating-coordinates-ellipse-in-inertial-coordinates-and-maxima-of-relative-speed). The oscillator's astroid in rotating coordinates, ellipse in inertial coordinates, and maxima of relative speed**.

## ↑ Ancestors (10)

1. [9A](../9a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
