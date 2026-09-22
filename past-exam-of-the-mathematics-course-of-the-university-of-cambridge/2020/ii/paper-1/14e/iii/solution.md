<h1 id="14e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since $1-C=1/2$, the [second local hypergeometric solution](../../../../../../second-local-hypergeometric-solution.md) is

$$
z^{1/2}F(A-C+1,B-C+1;2-C;z)
=z^{1/2}F\left(\frac{1+k}{2},\frac{1-k}{2};\frac32;z\right).
$$

Under $z=\sin^2x$, it must be a constant multiple of the independent elementary solution $\sin(kx)$. As $x\to0$, both $z^{1/2}$ and $x$ are asymptotic to one another, while $sin(kx)\sim kx$. Matching the normalized hypergeometric factor, whose value at zero is one, gives

$$
z^{1/2}F\left(\frac{1+k}{2},\frac{1-k}{2};\frac32;z\right)
=\frac{\sin(kx)}{k}.
$$

Consequently the [hypergeometric sine identity](../../../../../../hypergeometric-sine-identity.md) is

$$
\boxed{
F\left(\frac{1+k}{2},\frac{1-k}{2};\frac32;z\right)
=\frac{\sin\!\left(k\arcsin\sqrt z\right)}{k\sqrt z}
=\frac{\sin(kx)}{k\sin x}.
}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
