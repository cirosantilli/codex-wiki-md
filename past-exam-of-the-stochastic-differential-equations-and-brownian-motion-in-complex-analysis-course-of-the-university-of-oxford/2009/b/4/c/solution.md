<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Continuity and the regularity of zero for a one-dimensional Brownian coordinate make $S$ the first contact with the imaginary axis. The [Strong Markov property](../../../../../strong-markov-property.md) and symmetry of the subsequent real increments imply that reversing those increments after $S$ preserves the Brownian law. The imaginary coordinate is unchanged, so $\widetilde Z$ is again planar [Brownian motion](../../../../../brownian-motion-split.md) started at one.

Reflection preserves distance to the origin, hence $\widetilde T_{D_r}=T_{D_r}$ pathwise. On $T_{D_r}<S$, the path exits through the right semicircle and reflection has not yet acted. On $S<T_{D_r}$, reflection reverses the sign of the exit real part. Thus

$$
\mathbb P(\operatorname{Re}Z_T>0)
=\mathbb P(T<S)+\mathbb P(S<T,\operatorname{Re}Z_T>0),
$$



$$
\mathbb P(\operatorname{Re}\widetilde Z_T<0)
=\mathbb P(S<T,\operatorname{Re}Z_T>0).
$$

The two circular points on the imaginary axis have zero exit probability, so they cause no extra term. Subtracting proves the [reflection identity for Brownian exit from a half-disc](../../../../../reflection-identity-for-brownian-exit-from-a-half-disc.md) requested in the question.

Both processes have the same exit law. With $p=\pi^{-1}\tan^{-1}((r^2-1)/(2r))$ from part (b),

$$
\boxed{\mathbb P(T_{D_r}<S)=1-2p=\frac4\pi\tan^{-1}(1/r).}
$$

The final trigonometric identity follows from $\tan^{-1}((r^2-1)/(2r))=\pi/2-2\tan^{-1}(1/r)$ for $r>1$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
