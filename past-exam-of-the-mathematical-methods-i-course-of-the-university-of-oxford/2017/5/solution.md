<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [unit vector](../../../unit-vector.md), the radial coordinate is $r=1$ and the [spherical coordinates](../../../spherical-coordinate-system.md) give

$$
(n_x,n_y,n_z)=(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta).
$$

The [Pauli matrices](../../../pauli-matrices.md) therefore give

$$
\boxed{H=\begin{pmatrix}\cos\theta&e^{-i\phi}\sin\theta\\e^{i\phi}\sin\theta&-\cos\theta\end{pmatrix}.}
$$

The diagonal entries are real and the off-diagonal entries are [complex conjugates](../../../complex-conjugate.md), so $H^*=H$. Its trace is zero and its [determinant](../../../determinant.md) is $-1$, giving [eigenvalues](../../../eigenvalue.md) $+1$ and $-1$. A convenient [orthonormal eigenbasis](../../../orthonormal-eigenbasis.md) is

$$
\boxed{v_+=\binom{\cos(\theta/2)}{e^{i\phi}\sin(\theta/2)},\qquad
v_-=\binom{-\sin(\theta/2)}{e^{i\phi}\cos(\theta/2)}.}
$$

The half-angle identities verify $Hv_\pm=\pm v_\pm$, $v_\pm^*v_\pm=1$ and $v_+^*v_-=0$. Multiplication of either vector by any unit-modulus phase gives an equivalent normalized [eigenvector](../../../eigenvector.md). At a pole, the azimuth is undefined geometrically, but the remaining phase freedom makes the chosen expressions consistent with the same one-dimensional [eigenspaces](../../../eigenspace.md).

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2017](../../2017-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
