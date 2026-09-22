<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Given independent [primitive lattice translation vectors](../../../../primitive-lattice-translation-vector.md) $\mathbf a_1,\mathbf a_2,\mathbf a_3$, define

$$
V_p=\mathbf a_1\cdot(\mathbf a_2\times\mathbf a_3),\qquad
\mathbf b_1=2\pi\frac{\mathbf a_2\times\mathbf a_3}{V_p},\quad
\mathbf b_2=2\pi\frac{\mathbf a_3\times\mathbf a_1}{V_p},\quad
\mathbf b_3=2\pi\frac{\mathbf a_1\times\mathbf a_2}{V_p}.
$$

Then $\mathbf a_i\cdot\mathbf b_j=2\pi\delta_{ij}$. The [reciprocal lattice](../../../../reciprocal-lattice.md) consists of

$$
\boxed{\mathbf G=h\mathbf b_1+k\mathbf b_2+l\mathbf b_3,\qquad h,k,l\in\mathbb Z,}
$$

equivalently all [wavevectors](../../../../wavevector.md) for which $e^{i\mathbf G\cdot\mathbf R}=1$ for every direct [lattice vector](../../../../lattice-vector.md) $\mathbf R$.

For the [face-centered cubic lattice](../../../../face-centered-cubic-lattice.md), choose

$$
\mathbf a_1=\frac a2(0,1,1),\quad
\mathbf a_2=\frac a2(1,0,1),\quad
\mathbf a_3=\frac a2(1,1,0).
$$

Their [scalar triple product](../../../../scalar-triple-product.md) is $a^3/4$, and direct evaluation of the [cross products](../../../../cross-product.md) gives

$$
\mathbf b_1=\frac{2\pi}{a}(-1,1,1),\quad
\mathbf b_2=\frac{2\pi}{a}(1,-1,1),\quad
\mathbf b_3=\frac{2\pi}{a}(1,1,-1).
$$

Every integer combination has coordinates $(2\pi/a)(H,K,L)$ with $H,K,L$ all even or all odd. Conversely, for such coordinates the coefficients $(K+L)/2,(H+L)/2,(H+K)/2$ are integers, so every such point occurs. The even-coordinate points are the corners of cubes of edge $4\pi/a$, and the odd-coordinate points are their body centres. Therefore

$$
\boxed{\text{reciprocal Bravais lattice: body-centred cubic},\qquad a_{\rm reciprocal}=\frac{4\pi}{a}.}
$$

This is a property of the [Bravais lattice](../../../../bravais-lattice.md); the two-atom [atomic basis](../../../../atomic-basis-of-a-crystal.md) changes [structure factors](../../../../structure-factor.md) rather than these [reciprocal lattice](../../../../reciprocal-lattice.md) translation vectors.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
