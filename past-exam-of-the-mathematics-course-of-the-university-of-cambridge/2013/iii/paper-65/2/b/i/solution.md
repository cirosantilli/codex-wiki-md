<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $k>0$ without loss of generality, so $\alpha=kh/2>0$, and require decay as $Z\to\pm\infty$. The base velocity is $\tilde U=Z$ everywhere; there is no jump in its derivative. Let $C=\tilde c$ and $E=e^{-2\alpha}$. A decaying representation that already solves the layer equations is

$$
\tilde\psi=Ae^{-\alpha|Z+1|}+Be^{-\alpha|Z-1|}.
$$

It is continuous at both interfaces. At $Z=-1$ the value is $A+BE$ and the derivative jump is $-2\alpha A$; at $Z=1$ they are $B+AE$ and $-2\alpha B$. The density anomaly drops by one across each interface. The [jump conditions for stratified inviscid shear flow](../../../../../../../jump-conditions-for-stratified-inviscid-shear-flow.md) therefore reduce to

$$
\boxed{\begin{pmatrix}
2\alpha(1+C)^2-J&-JE\\
-JE&2\alpha(1-C)^2-J
\end{pmatrix}\begin{pmatrix}A\\B\end{pmatrix}=0.}
$$

For nonreal $C$ the displacement denominators do not vanish. Neutral limiting values are obtained by continuation, rather than by dividing by zero at an interface.

Set $q=J/(2\alpha)$. A nonzero mode requires the [determinant](../../../../../../../determinant.md) to vanish:

$$
[(1+C)^2-q][(1-C)^2-q]-q^2E^2=0.
$$

Expansion gives the [dispersion relation for two density interfaces in uniform shear](../../../../../../../dispersion-relation-for-two-density-interfaces-in-uniform-shear.md),

$$
\boxed{C^4-\left(2+\frac J\alpha\right)C^2+
\frac{(2\alpha-J)^2-J^2e^{-4\alpha}}{4\alpha^2}=0.}
$$

Uniform shear throughout the exterior is important: replacing it with constant exterior velocities would introduce [vorticity](../../../../../../../vorticity.md) jumps and give a different [dispersion relation](../../../../../../../dispersion-relation.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 65](../../../../paper-65-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
