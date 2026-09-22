<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At zero field the normalized [transfer matrix for a classical spin chain](../../../../transfer-matrix-for-a-classical-spin-chain.md) [eigenvectors](../../../../eigenvector.md) and [eigenvalues](../../../../eigenvalue.md) are

$$
\boxed{|+\rangle=\frac1{\sqrt2}\begin{pmatrix}1\\1\end{pmatrix},\quad
|-\rangle=\frac1{\sqrt2}\begin{pmatrix}1\\-1\end{pmatrix},\qquad
\lambda_+=2\cosh K,\quad\lambda_-=-2\sinh K.}
$$

The spin insertion exchanges the two [eigenvectors](../../../../eigenvector.md): $\sigma^z|+\rangle=|-\rangle$ and conversely. Evaluating the [trace](../../../../matrix-trace.md) in [c](../c.md) therefore gives, with $x=\lambda_-/\lambda_+=-\tanh K$,

$$
\boxed{g_N(r)=\frac{x^r+x^{N-r}}{1+x^N}.}
$$

This is the finite-ring result. In the [thermodynamic limit](../../../../thermodynamic-limit.md), or for $1\ll r\ll N$ away from the wrap-around image, it becomes

$$
\boxed{g(r)=(-\tanh\beta J)^r=(-1)^r e^{-r/\xi},\qquad
\xi=-\frac1{\log\tanh\beta J}.}
$$

Here $\xi$ is in lattice-site units. The alternating sign is antiferromagnetic order at short distances; the exponential envelope shows the absence of long-range order at every positive temperature in this one-dimensional finite-range model. As $T\to0$, $\xi$ diverges, asymptotically $\xi\sim\tfrac12e^{2\beta J}$. For the even ring the zero-temperature result is $g(r)=(-1)^r$, consistent with the two alternating ground configurations. At fixed finite $N$, “large distance” must still respect periodicity: $g_N(r)=g_N(N-r)$ rather than decaying indefinitely beyond the ring.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
