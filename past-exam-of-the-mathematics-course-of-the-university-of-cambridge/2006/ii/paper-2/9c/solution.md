<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

The [kinetic energy](../../../../../kinetic-energy.md) is $m(\dot\eta_1^2+\dot\eta_2^2)/2$. The Euler–Lagrange equations give

$$
m\ddot\eta_1=-(j+k)\eta_1+k\eta_2,\qquad m\ddot\eta_2=k\eta_1-(\ell+k)\eta_2.
$$

For a [normal mode](../../../../../normal-mode.md) $\eta=Ae^{i\omega t}$, the [stiffness matrix](../../../../../stiffness-matrix.md) is

$$
K=\begin{pmatrix}j+k&-k\\-k&\ell+k\end{pmatrix},\qquad \det(K-m\omega^2I)=0.
$$

Solving this quadratic yields

$$
\boxed{\omega_\pm^2=\frac{j+\ell+2k\pm\sqrt{(j-\ell)^2+4k^2}}{2m}.}
$$

Both are positive for positive spring constants. A corresponding amplitude ratio is $A_2/A_1=(j+k-m\omega_\pm^2)/k$; the lower-frequency mode has the masses moving in the same direction and the higher-frequency mode in opposite directions.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
