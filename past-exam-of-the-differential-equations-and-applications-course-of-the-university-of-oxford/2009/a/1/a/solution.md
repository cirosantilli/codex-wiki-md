<h1 id="a/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the auxiliary variable $y=\epsilon\dot x-x+x^3/3$. Differentiating gives $\dot y=\epsilon\ddot x+(x^2-1)\dot x=-x$, while rearrangement gives $\epsilon\dot x=x-x^3/3+y$. Conversely eliminating $y$ recovers the second-order equation, so this [phase plane](../../../../../phase-plane.md) system is equivalent. At an [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) $\dot y=0$ forces $x=0$, and the first equation then forces $y=0$. Its [Jacobian matrix](../../../../../jacobian-matrix.md) is

$$
J=\begin{pmatrix}\epsilon^{-1}&\epsilon^{-1}\\-1&0\end{pmatrix},\qquad\det(\lambda I-J)=\lambda^2-\epsilon^{-1}\lambda+\epsilon^{-1}.
$$

Thus $\epsilon\lambda^2-\lambda+1=0$. Expanding $\sqrt{1-4\epsilon}=1-2\epsilon-2\epsilon^2-4\epsilon^3+O(\epsilon^4)$ gives

$$
\boxed{\lambda_{\rm fast}=\epsilon^{-1}-1+O(\epsilon),\qquad\lambda_{\rm slow}=1+\epsilon+O(\epsilon^2).}
$$

For sufficiently small positive $\epsilon$ both are positive: the [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) is an [unstable node](../../../../../unstable-node.md). For negative $\epsilon$ the fast root is negative and the slow root positive, so it becomes a [saddle equilibrium](../../../../../saddle-equilibrium.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
