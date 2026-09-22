# First half-probability Grover iterate

↑ **Parent:** [Grover rotation angle](grover-rotation-angle.md)

If the marked fraction is $p$ and $\theta=\arcsin\sqrt p$, the success probability after $n$ [Grover search algorithm](grover-s-algorithm.md) iterations is $\sin^2((2n+1)\theta)$. For $0<p\leq1/2$, its first value at least $1/2$ occurs at

$$
n_{\min}=\left\lceil\frac{\pi}{8\theta}-\frac12\right\rceil.
$$

Before this integer the angle is below $\pi/4$, so success is below $1/2$. At this integer, the angle lies in $[\pi/4,\pi/4+2\theta)$, contained in $[\pi/4,3\pi/4)$, where squared sine is at least $1/2$. If $p\geq1/2$, no iteration is needed. For small $p$, $n_{\min}$ is asymptotic to $\pi/(8\sqrt p)$.

## ↑ Ancestors (6)

1. [Grover rotation angle](grover-rotation-angle.md)
2. [Grover's algorithm](grover-s-algorithm.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/2/b/solution.md)
