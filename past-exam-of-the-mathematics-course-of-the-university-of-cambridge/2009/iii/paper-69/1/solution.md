<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [modulus of continuity](../../../../../modulus-of-continuity.md) on the circle, $\omega(f,\delta)=\sup_{|h|\le\delta}\|f(\cdot+h)-f\|_\infty$. Splitting a displacement into steps of length at most $\delta$ and applying the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\omega(f,t)\le\left(1+\frac t\delta\right)\omega(f,\delta),\qquad t,\delta>0.
$$

The [Fejér kernel](../../../../../fejer-kernel.md) is nonnegative and has [integral](../../../../../integral.md) one, so

$$
\|\sigma_nf-f\|_\infty
\le\int_{-\pi}^{\pi}\omega(f,|t|)F_n(t)\,dt
\le\omega(f,\delta)\left(1+\frac1\delta\int_{-\pi}^{\pi}|t|F_n(t)\,dt\right).
$$

We therefore need its first absolute moment. The inequalities $|\sin(nt/2)|\le n|\sin(t/2)|$ and $\sin(|t|/2)\ge|t|/\pi$ on $[-\pi,\pi]$ imply

$$
0\le F_n(t)\le\min\left\{\frac{n}{2\pi},\frac{\pi}{2nt^2}\right\}.
$$

Splitting at $1/n$ gives

$$
\int_{-\pi}^{\pi}|t|F_n(t)\,dt
\le2\int_0^{1/n}t\frac{n}{2\pi}\,dt
+2\int_{1/n}^{\pi}t\frac{\pi}{2nt^2}\,dt
=\frac1{2\pi n}+\frac\pi n\ln(\pi n)
\le C\frac{\ln n}{n}\quad(n\ge2).
$$

Taking $\delta=\delta_n=(\ln n)/n$ in the preceding error bound proves the [Fejér first-moment approximation bound](../../../../../fejer-first-moment-approximation-bound.md):

$$
\boxed{\|\sigma_nf-f\|_\infty\le c\,\omega\left(f,\frac{\ln n}{n}\right),\qquad n\ge2.}
$$

The constants do not depend on $f$ or $n$. By the [Heine-Cantor theorem](../../../../../heine-cantor-theorem.md), a [continuous function](../../../../../continuous-function.md) on the compact circle is [uniformly continuous](../../../../../uniform-continuity.md), hence $\omega(f,\delta_n)\to0$ as $\delta_n\to0$. **Thus the Fejér sums converge uniformly to $f$.** The index restriction is necessary: at $n=1$ the printed scale is zero, while $\sigma_1f$ is the mean of $f$ and generally differs from it.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 69](../../paper-69-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
