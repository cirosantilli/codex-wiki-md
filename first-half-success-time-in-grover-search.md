# First half-success time in Grover search

↑ **Parent:** [Grover's algorithm](grover-s-algorithm.md)

For both oracle phases equal to $\pi$, the good/bad matrix is $\begin{pmatrix}\cos2\chi&\sin2\chi\\-\sin2\chi&\cos2\chi\end{pmatrix}$. Acting $r$ times on the initial vector $(\sin\chi,\cos\chi)$ yields success $\sin^2((2r+1)\chi)$. For $0<\chi\le\pi/4$, the first crossing of one half is the displayed integer, since the rounded angle stays between $\pi/4$ and $3\pi/4$. With $\sin^2\chi=m/N\ll1$ this is asymptotic to $(\pi/8)\sqrt{N/m}$. Iterating indefinitely is incorrect: the success oscillates after its first maximum.

## ↑ Ancestors (5)

1. [Grover's algorithm](grover-s-algorithm.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58/4/e/solution.md)
