<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Introduce the [slow time](../../../../../../../slow-time.md) $T=\epsilon t$ and use the [method of multiple scales](../../../../../../../method-of-multiple-scales.md) with $x_0=A(T)\cos\psi$, $\psi=t+\theta(T)$. The initial data give $A(0)=\sqrt2$ and $\theta(0)=-\pi/4$. At first order the equation for the correction is

$$
x_{1,tt}+x_1=2A'\sin\psi+2A\theta'\cos\psi+A f(A\cos\psi)\sin\psi.
$$

The [averaged amplitude for position-dependent damping](../../../../../../../averaged-amplitude-for-position-dependent-damping.md) follows from the [solvability condition in the method of multiple scales](../../../../../../../solvability-condition-in-the-method-of-multiple-scales.md), which removes the resonant sine and cosine terms. With brackets denoting a full-period average, this gives

$$
A'=-A\langle f(A\cos\psi)\sin^2\psi\rangle,\qquad\theta'=0.
$$

The [wave phase](../../../../../../../phase-waves.md) average vanishes because $f(A\cos\psi)\sin\psi\cos\psi$ changes sign under $\psi\mapsto2\pi-\psi$.

For the quadratic [position-dependent damping](../../../../../../../position-dependent-damping.md), $\langle\cos^2\psi\sin^2\psi\rangle=1/8$ and $\langle\sin^2\psi\rangle=1/2$, so

$$
A'=\frac A2-\frac{A^3}8,\qquad (A^2)'=A^2-\frac{A^4}4.
$$

Solving this [logistic equation](../../../../../../../logistic-differential-equation.md) with $A^2(0)=2$ gives $A(T)=2/\sqrt{1+e^{-T}}$. Thus **the uniformly valid leading approximation is**

$$
\boxed{x(t;\epsilon)=\frac{2\cos(t-\pi/4)}{\sqrt{1+e^{-\epsilon t}}}+O(\epsilon),
\qquad0\leq t\leq T_*/\epsilon.}
$$

Here $T_*$ is any fixed finite positive constant. Bounded nonresonant corrections and the averaging estimate make the error uniform on this slow-time interval. The leading expression meets the position datum exactly and the velocity datum to leading order; the first-order correction supplies its $O(\epsilon)$ adjustment.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 72](../../../../paper-72-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
