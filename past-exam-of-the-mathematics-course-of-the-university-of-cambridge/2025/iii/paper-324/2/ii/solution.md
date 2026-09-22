<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Normalization gives $p^2+q^2=1$. Write $p=\sin\theta$, $q=\cos\theta$ with $0<\theta<\pi/2$, and set $|u\rangle=U|b\rangle$. Define the two [Householder reflections](../../../../../../householder-transformation.md)

$$
R_u=2|u\rangle\langle u|-I
=U(2|b\rangle\langle b|-I)U^\dagger,
\qquad
R_\xi=I-2|\xi\rangle\langle\xi|.
$$

The [amplitude amplification](../../../../../../amplitude-amplification.md) iterate $G=R_uR_\xi$ preserves $\operatorname{span}\{|\xi\rangle,|\phi\rangle\}$ and rotates that plane through $2\theta$. Consequently

$$
\boxed{
G^kU|b\rangle
=\sin((2k+1)\theta)|\xi\rangle
+\cos((2k+1)\theta)|\phi\rangle}.
$$

In particular, $O(1/p)$ iterations raise the success probability to a constant close to one.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
