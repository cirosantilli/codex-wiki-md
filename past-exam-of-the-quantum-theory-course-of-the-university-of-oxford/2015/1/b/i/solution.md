<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In either exterior region of the [finite square well](../../../../../finite-square-well.md), the [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) reduces to $\psi''=k^2\psi$, since $E<0$. Its general solution is a [linear combination](../../../../../linear-combination.md) of $e^{kx}$ and $e^{-kx}$. On the left, $e^{-kx}$ grows as $x\to-\infty$ and cannot be a [square-integrable function](../../../../../square-integrable-function.md), so its coefficient must be zero. On the right, the excluded growing term is $e^{kx}$. Hence the surviving tails are $Ae^{kx}$ for $x\leq-a$ and $De^{-kx}$ for $x\geq a$.

Inside the well, $E+V_0>0$ and the equation becomes $\psi''=-\kappa^2\psi$, whose general solution is $B\cos\kappa x+C\sin\kappa x$. Thus

$$
\boxed{\psi(x)=\begin{cases}Ae^{kx},&x\leq-a,\\B\cos\kappa x+C\sin\kappa x,&-a<x<a,\\De^{-kx},&x\geq a.\end{cases}}
$$

The coefficients are initially independent; [wavefunction matching at a finite potential step](../../../../../wavefunction-matching-at-a-finite-potential-step.md) imposes the remaining relations. Here the paper's $k$ is the exterior decay constant and $\kappa$ is the interior oscillation constant.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
