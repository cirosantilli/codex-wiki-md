<h1 id="30a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put

$$
\alpha=\nu-\frac12,
\qquad
\chi=z-\frac{\pi\nu}{2}-\frac\pi4.
$$

The two endpoints $t=1$ and $t=-1$ both contribute. Near $t=1$, set $u=1-t$. Then

$$
(1-t^2)^{\nu-1/2}
=2^\alpha u^\alpha
\left(1-\frac u2\right)^\alpha,
\qquad
e^{izt}=e^{iz}e^{-izu}.
$$

Expanding the last amplitude in powers of $u$ and applying the [Complex Watson lemma](../../../../../../complex-watson-lemma.md) after rotating onto a decaying endpoint ray gives one exponential series. Repeating at $t=-1$ gives the other. After multiplication by the prefactor in the integral representation, the two endpoint contributions combine as

$$
J_\nu(z)
\sim\frac1{\sqrt{2\pi z}}
\left[
e^{i\chi}\sum_{k=0}^{\infty}\frac{i^ka_k(\nu)}{z^k}
+e^{-i\chi}\sum_{k=0}^{\infty}\frac{(-i)^ka_k(\nu)}{z^k}
\right],
$$

where

$$
a_k(\nu)
=\frac{\prod_{j=1}^k\left(4\nu^2-(2j-1)^2\right)}{k!8^k},
\qquad a_0=1.
$$

Separating the even and odd powers gives the [large-argument asymptotic expansion of the Bessel function of the first kind](../../../../../../large-argument-asymptotic-expansion-of-the-bessel-function-of-the-first-kind.md):

$$
\boxed{
J_\nu(z)\sim\sqrt{\frac2{\pi z}}
\left[
\cos\chi\sum_{m=0}^{\infty}
\frac{(-1)^ma_{2m}(\nu)}{z^{2m}}
-\sin\chi\sum_{m=0}^{\infty}
\frac{(-1)^ma_{2m+1}(\nu)}{z^{2m+1}}
\right].}
$$

Its first terms are

$$
J_\nu(z)\sim\sqrt{\frac2{\pi z}}
\left[
\cos\chi
-\frac{4\nu^2-1}{8z}\sin\chi
-\frac{(4\nu^2-1)(4\nu^2-9)}{2!(8z)^2}\cos\chi
+\cdots
\right].
$$

For fixed $\nu$, the expansion is uniform in every closed sector

$$
\boxed{|\arg z|\leq\pi-\delta}
$$

with $\delta>0$. The exclusion of the negative real axis fixes the branch of $z^{1/2}$ and stays away from its Stokes boundary.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [30A](../../30a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
