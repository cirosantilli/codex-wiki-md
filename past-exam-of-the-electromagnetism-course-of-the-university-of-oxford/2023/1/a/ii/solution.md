<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\mathbf n=\mathbf r/a$ be the [unit normal](../../../../../unit-normal.md) from the [electrical conductor](../../../../../electrical-conductor.md) into the [vacuum](../../../../../vacuum.md). The [electrostatic boundary conditions at a conductor](../../../../../electrostatic-boundary-conditions-at-a-conductor.md), together with the vanishing interior [electric field](../../../../../electric-field-split.md), give

$$
\boxed{\mathbf E_{\rm out}=\frac{\sigma}{\epsilon_0}\mathbf n,\qquad
\sigma=\epsilon_0\mathbf E_{\rm out}\cdot\mathbf n=-\epsilon_0\left.\partial_r\phi\right|_{a^+}.}
$$

Write $u=\cos\theta$ in [spherical coordinates](../../../../../spherical-coordinate-system.md), $D=|\mathbf r-\mathbf r_0|$ on $r=a$, and $z^\star=a^2/r_0$. Differentiating the [electric potential](../../../../../electric-potential.md) at fixed angles gives

$$
\left.\partial_r\phi\right|_{a^+}
=\frac q{4\pi\epsilon_0D^3}\left[-(a-r_0u)+\frac{r_0^2}{a^2}\left(a-\frac{a^2}{r_0}u\right)\right]
=\frac q{4\pi\epsilon_0D^3}\left(\frac{r_0^2}{a}-a\right).
$$

Here the distance identity in the preceding answer was used before simplifying. Hence the induced [surface charge density](../../../../../surface-charge-density.md) is

$$
\boxed{\sigma(\mathbf r)=\frac{q(a-r_0^2/a)}{4\pi|\mathbf r-\mathbf r_0|^3},\qquad |\mathbf r|=a.}
$$

For positive $q$ this [surface charge density](../../../../../surface-charge-density.md) is negative everywhere, with largest magnitude nearest the [point charge](../../../../../point-charge.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
