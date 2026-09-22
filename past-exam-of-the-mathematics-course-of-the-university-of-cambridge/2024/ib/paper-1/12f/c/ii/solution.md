<h1 id="12f/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put

$$
z_k=\frac1{a_k}=\frac{2}{(2k+1)\pi},
\qquad w=z-z_k.
$$

Near $a_k$, writing $\delta=1/z-a_k$ gives

$$
\tan(a_k+\delta)=-\cot\delta=-\frac1\delta+\frac\delta3+O(\delta^3).
$$

But

$$
\delta=\frac1z-\frac1{z_k}=-\frac{w}{z_k(z_k+w)},
$$

and hence, exactly,

$$
-\frac1\delta=\frac{z_k(z_k+w)}w=\frac{z_k^2}{w}+z_k.
$$

Since $\delta=O(w)$, the first two Laurent terms are

$$
\boxed{
\tan\frac1z
=\frac{z_k^2}{z-z_k}+z_k+O(z-z_k)}.
$$

Equivalently, substitute $z_k=2/((2k+1)\pi)$ in this expression.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [12F](../../../12f.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ib](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
