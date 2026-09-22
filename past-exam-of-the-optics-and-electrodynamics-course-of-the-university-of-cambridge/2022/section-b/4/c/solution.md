<h1 id="section-b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the first [polarizer](../../../../../polarizer.md)'s pass axis as $\mathbf e_1$ and write the second as $\mathbf a=(\mathbf e_1+\mathbf e_2)/\sqrt2$. The positive signed rotation takes $\mathbf e_1$ toward $\mathbf a$ by the short $\pi/4$ angle. Let $B_\parallel$ be signed according to $\theta=\Upsilon LB_\parallel$. The [Jones matrices](../../../../../jones-matrix.md) of ideal [polarizers](../../../../../polarizer.md) are their [orthogonal projection](../../../../../orthogonal-projection.md) matrices,

$$
P_1=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad
P_2=\mathbf a\mathbf a^{\mathsf T}=\frac12\begin{pmatrix}1&1\\1&1\end{pmatrix}.
$$

Removing the unimportant common propagation [phase](../../../../../phase-waves.md), the lossless glass block has the [rotation matrix](../../../../../rotation-matrix.md)

$$
R(\theta)=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}.
$$

The elements act from right to left, so

$$
\boxed{J_{S\to O}=P_2R(\theta)P_1
=\frac12\begin{pmatrix}\cos\theta+\sin\theta&0\\\cos\theta+\sin\theta&0\end{pmatrix},\qquad
\theta=\Upsilon LB_\parallel.}
$$

With the common optical [phase](../../../../../phase-waves.md) retained, multiply this by $e^{i\bar\phi}$. Extra scalar attenuation would also multiply the result, but none is supplied. A single [Jones vector](../../../../../jones-vector.md) does not represent [unpolarized light](../../../../../unpolarized-light.md); the device's [Jones matrix](../../../../../jones-matrix.md) is nevertheless well defined for each incident component and can be applied to their statistical mixture.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
