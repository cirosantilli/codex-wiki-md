<h1 id="12b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The coefficient matrix has [eigenvector](../../../../../../eigenvector.md) $u_+=(1,1)^T$ with eigenvalue $3$ and eigenvector $u_-=(1,-1)^T$ with eigenvalue $-1$. Write

$$
y(t)=p(t)u_++q(t)u_-.
$$

Since

$$
\begin{pmatrix}e^{2t}\\-2t\end{pmatrix}
=\frac{e^{2t}-2t}{2}u_+
+\frac{e^{2t}+2t}{2}u_-,
$$

and $y(0)=(1,-2)^T=-\tfrac12u_++\tfrac32u_-$, the system diagonalises to

$$
p'=3p+\frac{e^{2t}-2t}{2},\qquad p(0)=-\frac12,
$$



$$
q'=-q+\frac{e^{2t}+2t}{2},\qquad q(0)=\frac32.
$$

Using an [integrating factor](../../../../../../integrating-factor.md) gives

$$
p(t)=-\frac19e^{3t}-\frac12e^{2t}+\frac t3+\frac19,
$$



$$
q(t)=\frac16e^{2t}+t-1+\frac73e^{-t}.
$$

The unique fastest term is therefore

$$
y(t)=-\frac19e^{3t}u_++O(e^{2t}).
$$

Consequently $e^{-nt}y(t)$ diverges for $n<3$, tends to zero for $n>3$, and for $n=3$ tends to the finite nonzero vector

$$
\boxed{\lim_{t\to\infty}e^{-3t}y(t)
=-\frac19\begin{pmatrix}1\\1\end{pmatrix}}.
$$

Thus the only requested integer is

$$
\boxed{n=3}.
$$

This is an instance of [dominant eigenmode in a forced linear system](../../../../../../dominant-eigenmode-in-a-forced-linear-system.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12B](../../12b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
