<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the [Hadamard transform](../../../../hadamard-transform.md) to the conditional [quantum state](../../../../quantum-state.md) from [c](../c.md). Since $(x_k\oplus s)\cdot z=x_k\cdot z+s\cdot z$ modulo two, its output is

$$
H^{\otimes n}|\psi_k\rangle
=\frac1{\sqrt{2^{n+1}}}\sum_z(-1)^{x_k\cdot z}\bigl[1+(-1)^{s\cdot z}\bigr]|z\rangle.
$$

If $s\cdot z=1$, the two [probability amplitudes](../../../../probability-amplitude.md) cancel by destructive [quantum interference](../../../../quantum-interference.md). If $s\cdot z=0$, they add, giving

$$
\boxed{\Pr(z\mid k)=
\begin{cases}
2^{1-n},&z\cdot s=0,\\
0,&z\cdot s=1.
\end{cases}}
$$

Thus **every observed string obeys** $\boxed{z\cdot s=0}$. This [Simon Fourier sampling](../../../../simon-fourier-sampling.md) is uniform on the $(n-1)$-dimensional [vector subspace](../../../../vector-subspace.md) $s^\perp$ over the two-element [field](../../../../field.md). Indeed, the nonzero [linear functional](../../../../linear-functional.md) $z\mapsto z\cdot s$ has a [kernel](../../../../kernel-of-a-linear-map-split.md) of dimension $n-1$ by the [rank-nullity theorem](../../../../rank-nullity-theorem.md). The distribution does not depend on $k$, so measuring or discarding the second [quantum register](../../../../quantum-register.md) gives the same statistics for the first.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the introduction to quantum information course of the University of Oxford](../../../split.md)
5. [Introduction to quantum information course of the University of Oxford](../../../../introduction-to-quantum-information-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
