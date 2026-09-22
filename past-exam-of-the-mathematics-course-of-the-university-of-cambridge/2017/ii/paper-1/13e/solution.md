<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

For $\operatorname{Re}s>1$, expand $(e^t-1)^{-1}=\sum_{n\ge1}e^{-nt}$. Absolute integrability, bounded near zero by a constant times $t^{\operatorname{Re}s-2}$, permits termwise integration. The [Gamma function](../../../../../gamma-function.md) [integral](../../../../../integral.md) then gives

$$
\int_0^\infty\frac{t^{s-1}}{e^t-1}\,dt
=\sum_{n\ge1}n^{-s}\Gamma(s),
\qquad \boxed{\zeta_R(s)=\frac1{\Gamma(s)}\int_0^\infty\frac{t^{s-1}}{e^t-1}\,dt}.
$$

Specify the [Hankel contour](../../../../../hankel-contour.md) to run from the negative real axis below the cut towards zero, circle zero counterclockwise with fixed radius $0<r<2\pi$, and return above the cut. Take $-\pi<\arg t<\pi$. The circle excludes every nonzero pole $2\pi i\mathbb Z$ of the denominator. For $\operatorname{Re}s>1$ its radius can shrink to zero, and the lower and upper rays give respectively $-e^{-i\pi s}\Gamma(s)\zeta_R(s)$ and $e^{i\pi s}\Gamma(s)\zeta_R(s)$. By the [Gamma reflection formula](../../../../../gamma-reflection-formula.md),

$$
I(s)=\frac{\Gamma(1-s)\Gamma(s)\sin\pi s}{\pi}\zeta_R(s)=\zeta_R(s)
$$

away from integer $s$ in that half-plane, with limiting equality at the removable points.

With the circle radius kept fixed, the contour [integral](../../../../../integral.md) is an [entire function](../../../../../entire-function.md) of $s$: the rays decay exponentially and converge locally uniformly, and the circular part stays away from zero. Multiplication by $\Gamma(1-s)$ is analytic for $\operatorname{Re}s<1$ and meromorphic globally. The apparent singularities at positive integers $s\ge2$ are removable because the [integral](../../../../../integral.md) vanishes there and it already agrees with the original analytic zeta [function](../../../../../function-split.md) nearby. Only $s=1$ remains a simple pole. Thus this constructs the [meromorphic continuation](../../../../../meromorphic-continuation.md) to the whole plane and an [analytic continuation](../../../../../analytic-continuation.md) on $\mathbb C\setminus\{1\}$. Keeping the circular segment is essential when the [integral](../../../../../integral.md) is not locally integrable at zero.

At $s=-1$ the two rays cancel, since $t^{-2}$ is single-valued. The Laurent expansion

$$
\frac1{e^{-t}-1}=-\frac1t-\frac12-\frac t{12}+O(t^3)
$$

shows that the residue of $t^{-2}/(e^{-t}-1)$ is $-1/12$. Since $\Gamma(2)=1$, the [residue theorem](../../../../../residue-theorem.md) gives

$$
\boxed{\zeta_R(-1)=-\frac1{12}}.
$$

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
