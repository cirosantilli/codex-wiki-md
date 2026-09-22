<h1 id="2d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the single-frequency response, use [separation of variables](../../../../../../separation-of-variables.md) with $u=R(r)\sin\omega t$. Set $k=\omega/c$ and $V=rR$; then $V''+k^2V=0$, so $V=C\sin kr+D\cos kr$. A finite origin value forces $D=0$, since $\cos kr/r$ is singular. Since $\sin kr/r\to k$, the prescribed origin amplitude gives $C=A/k$. The [regular time-harmonic spherical wave](../../../../../../regular-time-harmonic-spherical-wave.md) is therefore

$$
\boxed{u(r,t)=A\frac{\sin(\omega r/c)}{\omega r/c}\sin\omega t},
$$

with the quotient defined by its limit at zero.

This answers the literal finite-origin condition in the class of regular single-frequency responses. It is a standing combination of inward and outward waves: the numerator is proportional to $\cos(kr-\omega t)-\cos(kr+\omega t)$. A purely outgoing wave from an ideal point source would instead be proportional to $r^{-1}\sin[\omega(t-r/c)]$, which has no finite prescribed value $u(0,t)$. Such a source must be specified by a singularity strength, for example $\lim_{r\downarrow0}ru$. The source's wording supplies neither an initial field nor an outgoing singular-source normalization; without restriction to the stated harmonic response, a general initial-value problem is not uniquely determined by the one origin condition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2D](../../2d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
