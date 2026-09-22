<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a separated solution $y=X(x)Q(t)$, the [wave equation](../../../../wave-equation-split.md) gives $X''/X=\ddot Q/(v^2Q)$. Choose the separation constant $-k^2$. Then

$$
X=A\cos kx+B\sin kx,\qquad Q=C\cos(vkt)+D\sin(vkt).
$$

These are the oscillatory separated building blocks. Since no endpoint conditions have yet been imposed, the general solution is a superposition over the allowed continuum of $k$, rather than one product with four constants. Equivalently, combining the left- and right-travelling separated components gives the [D'Alembert's formula](../../../../d-alembert-s-formula.md)

$$
\boxed{y(x,t)=F(x-vt)+G(x+vt),}
$$

with arbitrary twice differentiable functions $F,G$ on the relevant characteristic intervals. Indeed, in characteristic coordinates $\xi=x-vt$, $\eta=x+vt$, the equation becomes $y_{\xi\eta}=0$, whose general solution is exactly this sum. This also includes zero-frequency and polynomial limits that would be omitted by restricting to one nonzero-$k$ sine mode.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [2013 resit](../../../2013-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
