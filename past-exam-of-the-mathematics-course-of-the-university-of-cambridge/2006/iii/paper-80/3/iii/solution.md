<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\Delta=a_1-a_2<0$, and let $q=t\Delta\lambda\chi_1$. The inverse contrast in the [Hashin-Shtrikman conductivity variational principle](../../../../../../hashin-shtrikman-conductivity-variational-principle.md) is interpreted only in phase 1: the admissible $q$ vanishes in phase 2, where $a-a_2I=0$. Thus

$$
\mathbb E\!\left[2\lambda\cdot\int_\Omega q\,dx\right]
=2t\Delta p_1|\Omega||\lambda|^2,\qquad
\mathbb E\!\left[-\int_\Omega(a-a_2I)^{-1}q\cdot q\,dx\right]
=-t^2\Delta p_1|\Omega||\lambda|^2.
$$

For the nonlocal term define $K(x,x')=\nabla_x\nabla_{x'}g(x,x')$. The given Green representation implies

$$
\nabla v(x)=-\int_\Omega K(x,x')q(x')\,dx'.
$$

The [two-point phase correlation function](../../../../../../two-point-phase-correlation-function.md) therefore gives

$$
\mathbb E\int_\Omega q\cdot\nabla v\,dx
=-t^2\Delta^2\,\lambda\cdot
\left[\int_\Omega\int_\Omega p_{11}(|x-x'|)K(x,x')\,dx\,dx'\right]\lambda.
$$

Because the unweighted double integral of $K$ is zero, subtract $p_1^2$ inside the bracket. Set $h(r)=p_{11}(r)-p_1^2$; it vanishes for $r>\rho$, so only the microscopic near-diagonal kernel contributes. Its contact part is

$$
\frac{I}{3a_2}\delta(x-x').
$$

At coincident points $\chi_1^2=\chi_1$, hence $h(0)=p_1-p_1^2=p_1p_2$. The ordinary dipole part has zero angular integral by the stipulated spherical-shell identity. Since $h$ is radial, its weighting preserves this cancellation:

$$
\int_0^\rho h(r)\left[\int_{\partial B_r}H(s)\,dS_s\right]dr=0.
$$

Consequently, in the macroscopic bulk regime implicit in the supplied local Green approximation,

$$
\int_\Omega\int_\Omega p_{11}(|x-x'|)K(x,x')\,dx\,dx'
\simeq\frac{|\Omega|p_1p_2}{3a_2}I,
$$

and

$$
\mathbb E\int_\Omega q\cdot\nabla v\,dx
\simeq-\frac{t^2\Delta^2p_1p_2}{3a_2}|\Omega||\lambda|^2.
$$

This is the [dipole Green tensor angular cancellation](../../../../../../dipole-green-tensor-angular-cancellation.md): the constant background correlation disappears and the connected contact value supplies $p_1p_2$.

Insert all three averaged terms in the variational upper inequality and normalize by $|\Omega||\lambda|^2$. For the bulk [effective conductivity](../../../../../../effective-conductivity.md) one obtains

$$
\boxed{
a^*\le a_2+\Delta p_1\left[2t-t^2\left(1+\frac{\Delta p_2}{3a_2}\right)\right].
}
$$

The kernel in the question has an approximation sign. At fixed finite size, [spheres](../../../../../../sphere.md) around points near $\partial\Omega$ are truncated and the radial cancellation is not an exact finite-body identity. Their contribution and the regular boundary part disappear in the stated microscopic-to-macroscopic limit. The calculation derives the intended homogenized bound, rather than silently treating that Green approximation as exact for arbitrary finite $\rho$.

Let $C=1+\Delta p_2/(3a_2)$. Since $a_1>0$, $\Delta>-a_2$, so $C>0$. Also $\Delta p_1<0$ when both phases are present. Completing the square in the trial upper bound gives

$$
a_2+\Delta p_1(2t-Ct^2)
=a_2+\frac{\Delta p_1}{C}-\Delta p_1C\left(t-\frac1C\right)^2.
$$

Thus the tightest upper bound is obtained by minimizing at $t=1/C$, not maximizing. It is

$$
\boxed{
a^*\le a_2+\frac{3a_2(a_1-a_2)p_1}{3a_2+p_2(a_1-a_2)}.
}
$$

Pure-phase cases follow directly or by continuity. These [Hashin-Shtrikman bounds for conductivity](../../../../../../hashin-shtrikman-bounds-for-conductivity.md) are volume-fraction bounds on the statistically [isotropic](../../../../../../isotropy.md) homogenized material; the full variational framework is discussed in Chapter 23 of [https://www.math.utah.edu/~milton/TheoryCompositesNOPRINT.pdf](https://www.math.utah.edu/~milton/TheoryCompositesNOPRINT.pdf) .

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
