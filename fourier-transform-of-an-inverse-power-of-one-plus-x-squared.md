# Fourier transform of an inverse power of one plus x squared

↑ **Parent:** [Fourier transform](fourier-transform-split.md)

For $\alpha>0$, put $a=\alpha/2$. The [regular distribution](regular-distribution.md) of $(1+x^2)^{-a}$ is a [tempered distribution](tempered-distribution.md), since the [function](function-split.md) is bounded. Its [Fourier transform](fourier-transform-split.md) is the [integrable function](lebesgue-integrable-function.md)

$$
h_\alpha(\xi)=\frac{\sqrt\pi}{\Gamma(a)}\int_0^\infty t^{a-3/2}e^{-t-\xi^2/(4t)}\,dt\qquad(\xi\ne0),
$$

with arbitrary finite value at zero when the displayed [integral](integral-split.md) diverges there. To prove the identity, the [gamma function](gamma-function.md) gives $(1+x^2)^{-a}=\Gamma(a)^{-1}\int_0^\infty t^{a-1}e^{-t}e^{-tx^2}\,dt$. Pair this with a [Schwartz function](schwartz-function.md), use the [Fourier transform of a Gaussian](fourier-transform-of-a-gaussian.md), and interchange [integrals](integral-split.md) by [Fubini's theorem](fubini-s-theorem.md). The absolute bound for the transformed pairing follows from [Tonelli's theorem](tonelli-theorem.md):

$$
\|h_\alpha\|_1=\frac{\sqrt\pi}{\Gamma(a)}\int_0^\infty t^{a-3/2}e^{-t}\,2\sqrt{\pi t}\,dt=2\pi.
$$

The positive kernel and [dominated convergence](dominated-convergence-theorem.md) give positivity and continuity away from zero. It has a continuous representative at zero exactly when $\alpha>1$, in which case $h_\alpha(0)=\sqrt\pi\Gamma((\alpha-1)/2)/\Gamma(\alpha/2)$. For $\alpha\leq1$, [Fatou's lemma](fatou-s-lemma.md) gives $h_\alpha(\xi)\to\infty$ as $\xi\to0$, so no change on a set of zero [Lebesgue measure](lebesgue-measure.md) can give continuity.

## ↑ Ancestors (5)

1. [Fourier transform](fourier-transform-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/1/b/i/solution.md)
