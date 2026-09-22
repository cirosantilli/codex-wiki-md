<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

Let the [Bravais lattice](../../../../../bravais-lattice.md) have primitive vectors $a_1,a_2,a_3$, and put

$$
\Omega=a_1\cdot(a_2\times a_3).
$$

The [reciprocal lattice](../../../../../reciprocal-lattice.md) has the [basis](../../../../../basis.md)

$$
b_1=2\pi\frac{a_2\times a_3}{\Omega},\qquad
b_2=2\pi\frac{a_3\times a_1}{\Omega},\qquad
b_3=2\pi\frac{a_1\times a_2}{\Omega}.
$$

The [scalar triple product](../../../../../scalar-triple-product.md) and [cross product](../../../../../cross-product.md) identities give

$$
a_i\cdot b_j=2\pi\delta_{ij}.
$$

Consequently every $q=\sum_jn_jb_j$ satisfies $q\cdot l\in2\pi\mathbb Z$ for every [lattice point](../../../../../lattice-point.md) $l=\sum_im_ia_i$, and conversely these three conditions force the coefficients of $q$ in the reciprocal basis to be [integers](../../../../../integer.md). This proves that the displayed vectors generate $\Lambda^*$.

In the [Born approximation](../../../../../born-approximation.md), suppose that the crystal potential is the [sum](../../../../../sum.md) of translates of one atomic potential $V_0$ over the finite set $S$ of lattice sites. Its [Fourier transform](../../../../../fourier-transform.md) at the [momentum transfer](../../../../../momentum-transfer.md) $Q=k-k'$ factors as

$$
\widetilde V(Q)=\widetilde V_0(Q)\Delta(Q),
\qquad
\Delta(Q)=\sum_{l\in S}e^{iQ\cdot l}.
$$

Thus the single-atom [scattering amplitude](../../../../../scattering-amplitude.md) is multiplied by the [crystal lattice structure factor](../../../../../crystal-lattice-structure-factor.md) $\Delta(Q)$. Writing

$$
l=l_1a_1+l_2a_2+l_3a_3,
\qquad
\alpha_i=Q\cdot a_i,
$$

separates the sum into three [finite geometric series](../../../../../finite-geometric-series.md). For $l_i=-L_i/2,\ldots,L_i/2$ this gives

$$
\boxed{
\Delta(Q)=\prod_{i=1}^3
\frac{\sin((L_i+1)\alpha_i/2)}{\sin(\alpha_i/2)}.}
$$

When the $L_i$ are large, a factor has a sharp maximum when $\alpha_i=2\pi n_i$. All three factors are therefore simultaneously large precisely when $Q\in\Lambda^*$. These are the [reciprocal-lattice peaks of a finite crystal](../../../../../reciprocal-lattice-peaks-of-a-finite-crystal.md).

For the stated [body-centered cubic lattice](../../../../../body-centered-cubic-lattice.md) basis,

$$
a_1=\frac a2(1,1,1),\qquad
a_2=\frac a2(1,-1,1),\qquad
a_3=a(0,0,1),
$$

the reciprocal-basis formula gives

$$
b_1=\frac{2\pi}{a}(1,1,0),\qquad
b_2=\frac{2\pi}{a}(1,-1,0),\qquad
b_3=\frac{2\pi}{a}(-1,0,1).
$$

Equivalently,

$$
\Lambda^*=\frac{2\pi}{a}
\{(h,k,l)\in\mathbb Z^3:h+k+l\text{ is even}\}.
$$

The shortest nonzero reciprocal vectors have squared [Euclidean norm](../../../../../euclidean-norm.md) $2(2\pi/a)^2$, so

$$
q_{\min}=\frac{2\sqrt2\pi}{a}.
$$

In [elastic scattering](../../../../../elastic-scattering.md), $|k|=|k'|=k$. If $q=k-k'\in\Lambda^*$ and $\theta$ is the angle between $k$ and $k'$, [Euclidean geometry](../../../../../euclidean-geometry.md) gives

$$
|q|=2k\sin\frac\theta2.
$$

The first possible [diffraction](../../../../../diffraction.md) peak therefore occurs at

$$
\boxed{
\theta_{\min}=2\arcsin\!\left(\frac{\sqrt2\pi}{ka}\right)
\sim\frac{2\sqrt2\pi}{ka}}
$$

as $ka\to\infty$, by the [small-angle approximation](../../../../../small-angle-approximation.md). This is the [elastic Bragg scattering condition](../../../../../elastic-bragg-scattering-condition.md) for the shortest reciprocal-lattice vector.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
