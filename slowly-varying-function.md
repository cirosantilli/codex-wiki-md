# Slowly varying function

↑ **Parent:** [Regular variation](regular-variation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slowly_varying_function)

A positive [measurable function](measurable-function.md) $\ell$ is slowly varying at infinity if

$$
\frac{\ell(ut)}{\ell(t)}\longrightarrow1
\qquad(t\to\infty)
$$

for every fixed $u>0$. It has [regular variation](regular-variation.md) of index zero. “Slowly” concerns relative change under multiplication of the argument; it does not mean that the [function](function-split.md) must be bounded, have a small [derivative](derivative.md), or converge to a finite value.

Every positive constant is a [slowly varying function](slowly-varying-function.md). So are $\log t$, $1/\log t$ and $(\log t)^a$ for any fixed [real number](real-number.md) $a$, on $t>1$. Indeed,

$$
\frac{(\log(ut))^a}{(\log t)^a}
=\left(1+\frac{\log u}{\log t}\right)^a\longrightarrow1.
$$

The first grows without bound, the second tends to zero, and the constant does neither. Another unbounded example is $\ell(t)=e^{\sqrt{\log t}}$:

$$
\log\frac{\ell(ut)}{\ell(t)}
=\frac{\log u}{\sqrt{\log t+\log u}+\sqrt{\log t}}
\longrightarrow0.
$$

This [function](function-split.md) can grow much faster than $\log t$ while retaining [regular variation](regular-variation.md) of index zero.

Even convergence is unnecessary. The bounded [function](function-split.md)

$$
\ell(t)=\exp\!\bigl(\sin(\log\log t)\bigr),\qquad t>1,
$$

oscillates between $e^{-1}$ and $e$. It is nevertheless a [slowly varying function](slowly-varying-function.md): the change in the argument of the [sine](sine.md) under $t\mapsto ut$ is

$$
\log\log(ut)-\log\log t
=\log\left(1+\frac{\log u}{\log t}\right)\longrightarrow0,
$$

and the [Lipschitz continuity](lipschitz-continuity.md) of the [sine](sine.md) makes the logarithm of the ratio tend to zero. The [sequences](sequence.md) $t_k=\exp(\exp(\pi/2+2\pi k))$ and $s_k=\exp(\exp(3\pi/2+2\pi k))$ give the two values $e$ and $e^{-1}$ for every nonnegative [integer](integer.md) $k$, so there is no [limit](limit-of-a-function.md) at infinity.

Contrast this with $h(t)=2+\sin(\log t)$, which is positive and bounded but is not a [slowly varying function](slowly-varying-function.md). Fix $u=e^{\pi/2}$. Along $t_k=e^{2\pi k}$ its rescaling ratio is $h(ut_k)/h(t_k)=3/2$; along $s_k=e^{\pi+2\pi k}$ the ratio is $1/2$. The persistent oscillations prevent even a [limit](limit-of-a-function.md) for this one fixed rescaling. It is not [regularly varying](regular-variation.md) with any finite index either.

<a id="image-two-bounded-oscillating-functions-logarithmic-rescaling-makes-one-ratio-approach-one-while-the-other-keeps-oscillating"></a>
![](slow-variation-oscillation-comparison.png)

**[Figure 7](#image-two-bounded-oscillating-functions-logarithmic-rescaling-makes-one-ratio-approach-one-while-the-other-keeps-oscillating). Two bounded oscillating functions: logarithmic rescaling makes one ratio approach one, while the other keeps oscillating**. The horizontal coordinate is $s=\log t$, and the fixed rescaling is $u=e^{\pi/2}$. The displayed range illustrates the formulas; the limiting claims follow from the arguments in the text.

The useful distinction is whether a fixed proportional change of input eventually produces a negligible proportional change of output. A [slowly varying function](slowly-varying-function.md) can therefore preserve the scaling exponent of a [power law](power-law.md) while changing its magnitude substantially. The decomposition in [regular variation](regular-variation.md) explains why a logarithmic factor can matter in numerical estimates without changing the limiting exponent.

## ↑ Ancestors (6)

1. [Regular variation](regular-variation.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/3/solution.md)
- [Regular variation](regular-variation.md)
- [Slowly varying function](slowly-varying-function.md)
