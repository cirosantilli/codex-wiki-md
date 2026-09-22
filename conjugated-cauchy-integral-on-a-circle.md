# Conjugated Cauchy integral on a circle

↑ **Parent:** [Cauchy integral formula](cauchy-integral-formula.md)

If $f$ is [holomorphic](holomorphic-function-split.md) on a neighborhood of the closed [unit disc](unit-disc.md) and $|a|<1$, this boundary integral is independent of $a$. Parametrizing the [unit circle](complex-unit-circle.md) by $z=e^{it}$ and taking a [complex conjugate](complex-conjugate.md) gives

$$
\overline{\frac1{2\pi i}\int_{|z|=1}\frac{\overline{f(z)}}{z-a}\,dz}
=\frac1{2\pi i}\int_{|z|=1}\frac{f(z)}{z(1-\overline a z)}\,dz=f(0),
$$

where the last equality is the [Cauchy integral formula](cauchy-integral-formula.md) applied to the [holomorphic function](holomorphic-function-split.md) $f(z)/(1-\overline a z)$ at zero. The conjugation of the whole integral includes the factor $1/i$ and the differential; parametrization keeps their signs consistent. Equivalently, the conjugated boundary values have only nonpositive Fourier frequencies, so the Cauchy kernel detects their constant coefficient.

## ↑ Ancestors (5)

1. [Cauchy integral formula](cauchy-integral-formula.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-analysis-and-differential-equations-2-course-of-the-university-of-oxford/2007/4/solution.md)
