# Semidiscrete fixed-string normal mode

↑ **Parent:** [Wave equation on a string](wave-equation-on-a-string.md)

The [second-order central difference](second-order-central-difference.md) approximation to the fixed-end [wave equation](wave-equation-split.md) on $n$ interior points has [normal modes](normal-mode.md)

$$
v_j^{(k)}=\sqrt{\frac2{n+1}}\sin\frac{jk\pi}{n+1},\qquad
\lambda_k=-\frac{4c^2}{h^2}\sin^2\frac{k\pi}{2(n+1)},\qquad
\omega_k=\sqrt{-\lambda_k},\qquad 1\le j,k\le n.
$$

Here $h=L/(n+1)$ and the endpoint [displacements](displacement.md) are zero. The [eigenvectors](eigenvector.md) form an [orthonormal basis](orthonormal-basis.md) in the ordinary [Euclidean norm](euclidean-norm.md), without an extra grid-spacing weight. They sample the continuous [standing wave](standing-wave.md) shapes exactly, while their [angular frequencies](angular-frequency.md) differ from $k\pi c/L$ because of spatial discretization. For fixed $k$, the difference tends to zero as $h\to0$.

## ↑ Ancestors (7)

1. [Wave equation on a string](wave-equation-on-a-string.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford/2024/paper-3/5/e/solution.md)
