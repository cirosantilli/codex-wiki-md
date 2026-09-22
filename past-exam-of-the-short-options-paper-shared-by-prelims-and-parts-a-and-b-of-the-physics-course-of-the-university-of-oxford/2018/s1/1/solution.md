<h1 id="s1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [branch point](../../../../branch-point.md) is a point around which [analytic continuation](../../../../analytic-continuation.md) changes the value of a multivalued function. For $z^{1/2}=r^{1/2}e^{i\theta/2}$, one circuit around zero changes the sign. A [branch cut](../../../../branch-cut.md) removes paths producing this ambiguity; for example $-\pi<\arg z<\pi$ gives a single holomorphic [square root](../../../../square-root.md) off the nonpositive [real axis](../../../../real-axis.md). The [position](../../../../position.md) of a cut is a convention, while the [branch point](../../../../branch-point.md) is intrinsic.

Set $q(z)=(z-1)/(z+1)$. For $z$ outside the closed segment joining $-1$ to $1$, $q(z)$ avoids the nonpositive [real axis](../../../../real-axis.md). Therefore the [principal square root](../../../../principal-square-root-of-a-complex-number.md) of $q$ defines a [holomorphic function](../../../../holomorphic-function-split.md) there, with the [normalization](../../../../normalization.md) $f(\infty)=1$. The endpoints are [branch points](../../../../branch-point.md). Expanding at infinity,

$$
f(z)=\left(1-\frac2{z+1}\right)^{1/2}=1-\frac1z+O(z^{-2}).
$$

For a positively oriented contour surrounding the cut, its [integral](../../../../integral-split.md) equals the [integral](../../../../integral-split.md) on a sufficiently large positively oriented circle, since the intervening annulus is holomorphic. Thus

$$
\boxed{I_\Gamma=-2\pi i.}
$$

On the upper and lower banks, $f_+(x)=+i\sqrt{(1-x)/(1+x)}$ and $f_-(x)=-i\sqrt{(1-x)/(1+x)}$. The upper bank is traversed from $1$ to $-1$, and the lower bank from $-1$ to $1$. Their sum is $-2i$ [times](../../../../time-in-physics.md) the required real [integral](../../../../integral-split.md). Small endpoint arcs vanish because their singularities have exponent less than one. Consequently

$$
\boxed{\int_{-1}^{1}\sqrt{\frac{1-x}{1+x}}\,dx=\pi.}
$$

For $\alpha=1/n$, use $f_\alpha=q^\alpha$ with the same [normalization](../../../../normalization.md). Its expansion is $1-2\alpha/z+O(z^{-2})$, and its bank values are $e^{\pm i\pi\alpha}[(1-x)/(1+x)]^\alpha$. Equating the [contour integral](../../../../contour-integral.md) $-4\pi i\alpha$ with $-2i\sin(\pi\alpha)$ [times](../../../../time-in-physics.md) the real [integral](../../../../integral-split.md) gives

$$
\boxed{\int_{-1}^{1}\left(\frac{1-x}{1+x}\right)^{1/n}dx
=\frac{2\pi}{n\sin(\pi/n)}.}
$$

The condition $n\ge2$ ensures endpoint integrability. Choosing the other square-root branch reverses $I_\Gamma$, but also reverses both bank values, leaving the real [integral](../../../../integral-split.md) unchanged.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [S1](../../s1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../split.md)
5. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
