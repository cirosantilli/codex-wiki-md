<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [Jacobian matrix](../../../../../jacobian-matrix.md) of the update map is

$$
J(H,P)=\begin{pmatrix}
r e^{-aP}&-arHe^{-aP}\\
b(1-e^{-aP})&abHe^{-aP}
\end{pmatrix},\qquad
J(0,0)=\begin{pmatrix}r&0\\0&0\end{pmatrix}.
$$

Its [eigenvalues](../../../../../eigenvalue.md) are $r$ and zero. The extinction [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) is locally [asymptotically stable](../../../../../asymptotic-stability.md) for $0<r<1$ and unstable for $r>1$, by [linear stability analysis](../../../../../linear-stability.md) for a [discrete dynamical system](../../../../../discrete-dynamical-system-split.md). In the latter case, even a small perturbation along $P=0$ grows as $H_t=r^tH_0$.

At $r=1$, an [eigenvalue](../../../../../eigenvalue.md) equals one, so the strict linear criterion does not decide stability. Directly, $0\le H_{t+1}\le H_t$ and $0\le P_{t+1}\le bH_t$. Starting sufficiently close to extinction therefore keeps both coordinates close for all time, proving [Lyapunov stability](../../../../../lyapunov-stability.md) in the nonnegative state space. It is not [asymptotically stable](../../../../../asymptotic-stability.md), since every nearby $(H,0)$ is another [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md). This distinction makes the statement “stable when $r>1$ fails” precise.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
