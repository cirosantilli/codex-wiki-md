<h1 id="19g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Normalize [Haar measure](../../../../../../haar-measure.md) on $\mathrm{SU}(2)$ to total mass one. For a [continuous](../../../../../../continuous-function.md) class function $F$, the [Weyl integration formula for SU2](../../../../../../weyl-integration-formula-for-su-2.md) is

$$
\boxed{\int_{\mathrm{SU}(2)}F(g)\,dg
=\frac2\pi\int_0^\pi
F(\operatorname{diag}(e^{i\theta},e^{-i\theta}))\sin^2\theta\,d\theta}.
$$

Equivalently it is $\pi^{-1}\int_0^{2\pi}F(t_\theta)\sin^2\theta\,d\theta$. For arbitrary [continuous](../../../../../../continuous-function.md) $F$, replace $F(t_\theta)$ on the right by its conjugacy average $\int_{\mathrm{SU}(2)}F(ht_\theta h^{-1})\,dh$.

Here is a direct proof. Identify $\mathrm{SU}(2)$ with unit quaternions, the sphere $S^3$. Multiplication by a unit quaternion is a transformation given by an [orthogonal matrix](../../../../../../orthogonal-matrix.md) of $\mathbb R^4$, so normalized round volume is bi-invariant and is [Haar measure](../../../../../../haar-measure.md). Write a quaternion as $\cos\theta+\mathbf n\sin\theta$, $0\le\theta\le\pi$, $\mathbf n\in S^2$. The round volume element is $\sin^2\theta\,d\theta\,dA(\mathbf n)$, and the total volume is $2\pi^2$. Conjugation rotates the unit imaginary [vector](../../../../../../vector.md) $\mathbf n$, so a class function depends only on $\theta$. Integrating over the sphere of area $4\pi$ gives the factor $4\pi/(2\pi^2)=2/\pi$. The endpoint degeneracies have measure zero. Conjugacy averaging and Haar invariance prove the more general version.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [19G](../../19g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
