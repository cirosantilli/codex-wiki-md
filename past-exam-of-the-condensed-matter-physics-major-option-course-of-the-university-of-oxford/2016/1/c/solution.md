<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $F_x(\mathbf h)=f_x S_x(h,k,l)$, where the four-site orbit has [structure factor](../../../../structure-factor.md)

$$
\begin{aligned}
S_x(h,k,l)={}&e^{2\pi ix(h+k+l)}+(-1)^{h+l}e^{2\pi ix(-h-k+l)}\\
&+(-1)^{k+l}e^{2\pi ix(-h+k-l)}+(-1)^{h+k}e^{2\pi ix(h-k-l)}.
\end{aligned}
$$

A cyclic permutation of $h,k,l$ fixes the first term and permutes the remaining three. Thus $S_x(k,l,h)=S_x(h,k,l)$. Substituting $-h,-k,l$ exchanges the first and second exponentials and the third and fourth, with the common coefficient $(-1)^{h+l}$:

$$
\boxed{S_x(-h,-k,l)=e^{-i\pi(h+l)}S_x(h,k,l)}.
$$

The two forms of this phase, $e^{+i\pi(h+l)}$ and $e^{-i\pi(h+l)}$, agree for integer indices. Multiplication by a unit-modulus phase preserves intensity, irrespective of whether $f_x$ is real or complex. Since the phase is independent of $x$ and atomic species, it also multiplies the total [structure factor](../../../../structure-factor.md) of the crystal.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
