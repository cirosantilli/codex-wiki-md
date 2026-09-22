<h1 id="34b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Now $g=1$, so $c=\langle\psi|\phi\rangle$ is real and

$$
|\pm\rangle=\frac{|\psi\rangle\pm|\phi\rangle}
 {\sqrt{2(1\pm c)}}.
$$

The perturbation is diagonal in this [basis](../../../../../../basis.md):

$$
\Delta(t)|+\rangle=2V(t)|+\rangle,
\qquad
\Delta(t)|-\rangle=0.
$$

Hence the instantaneous [eigenvalues](../../../../../../eigenvalue.md) are $1+2V(t)$ and $-1$ with time-independent [eigenvectors](../../../../../../eigenvector.md), so [Hamiltonians](../../../../../../hamiltonian.md) at different times commute. In units $\hbar=1$, put

$$
W(t)=\int_0^tV(s)\,ds.
$$

Expanding the initial state and evolving its two components gives

$$
|\psi(t)\rangle
=\frac{\sqrt{2(1+c)}}2e^{-i[t+2W(t)]}|+\rangle
 +\frac{\sqrt{2(1-c)}}2e^{it}|-\rangle.
$$

Taking its overlap with $|\phi\rangle$ and simplifying gives the exact transition probability

$$
\boxed{
\mathbb P_{\psi\to\phi}(t)
=c^2+(1-c^2)\sin^2\!\bigl(t+W(t)\bigr).}
$$

With explicit $\hbar$, each phase in the final sine is divided by $\hbar$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [34B](../../34b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
