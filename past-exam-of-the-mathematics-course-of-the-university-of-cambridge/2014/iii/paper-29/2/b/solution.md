<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $E_+$ and $E_-$ denote positive and negative real part at the circular exit. On $\{S<T(r)\}$, reflect the portion of the [planar Brownian motion](../../../../../../planar-brownian-motion.md) after $S$ by $z\mapsto-\overline z$. This reflection fixes the imaginary axis and preserves distances from the origin. The [Strong Markov property](../../../../../../strong-markov-property.md) and reflection symmetry show that the resulting path has the same law, its circular exit time is unchanged, and $E_+$ is exchanged with $E_-$. Therefore

$$
\mathbb P_1(S<T(r),E_+)=\mathbb P_1(S<T(r),E_-).
$$

An exit with negative real part must first cross the imaginary axis. An exit before $S$ has positive real part. The two points $ir,-ir$ have zero circular exit probability, since circular [harmonic measure](../../../../../../harmonic-measure.md) has no atoms. Hence

$$
\begin{aligned}
\mathbb P_1(E_+)&=\mathbb P_1(T(r)<S)+\mathbb P_1(S<T(r),E_+),\\
\mathbb P_1(E_-)&=\mathbb P_1(S<T(r),E_-).
\end{aligned}
$$

Subtracting proves

$$
\boxed{\mathbb P_1(T(r)<S)=\mathbb P_1(E_+)-\mathbb P_1(E_-).}
$$

This is the [reflection identity for Brownian exit from a half-disc](../../../../../../reflection-identity-for-brownian-exit-from-a-half-disc.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
