<h1 id="33e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Since $L^T=L$ and $B^T=-B$,

$$
[B,L]^T=(BL-LB)^T=L(-B)-(-B)L=[B,L],
$$

so the commutator is symmetric. If $Lv=\lambda v$ with $\lVert v\rVert=1$, symmetry permits a differentiable orthonormal eigenbasis locally, and

$$
\dot\lambda=v^T\dot Lv
=v^T(BL-LB)v
=\lambda v^TBv-\lambda v^TBv=0.
$$

Thus a [Lax pair](../../../../../../lax-pair.md) evolution is [isospectral](../../../../../../isospectral-lax-equation.md).

For the harmonic oscillator,

$$
H(q,p)=\frac12(p^2+\omega^2q^2),\qquad
\dot q=p,\qquad \dot p=-\omega^2q.
$$

With the stated $L$, take

$$
B=\begin{pmatrix}0&-\omega/2\\ \omega/2&0\end{pmatrix}.
$$

Direct calculation gives

$$
[B,L]=
\begin{pmatrix}-\omega^2q&\omega p\\
\omega p&\omega^2q\end{pmatrix}
=\dot L.
$$

The eigenvalues of $L$ are

$$
\lambda_\pm=\pm\sqrt{p^2+\omega^2q^2}.
$$

Their constancy proves conservation of the oscillator energy $H=\lambda_+^2/2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [33E](../../33e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
