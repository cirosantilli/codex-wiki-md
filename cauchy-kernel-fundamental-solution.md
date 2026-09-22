# Cauchy kernel fundamental solution

↑ **Parent:** [Fundamental solution of a linear differential operator](fundamental-solution-of-a-linear-differential-operator.md)

The [locally integrable function](locally-integrable-function.md) $E(z)=1/(\pi z)$ on the plane is a [fundamental solution](fundamental-solution-of-a-linear-differential-operator.md) for the [Wirtinger derivative](wirtinger-derivatives.md) $\partial_{\bar z}=(\partial_x+i\partial_y)/2$. Let $L=(4\pi)^{-1}\log(x^2+y^2)$ be the [fundamental solution of the Laplace equation](fundamental-solution-of-the-laplace-equation.md). Its first [distributional derivatives](distributional-derivative.md) agree with its ordinary ones: deleting a radius-$\varepsilon$ disk in [integration by parts](integration-by-parts.md) gives an error $O(\varepsilon|\log\varepsilon|)$, tending to zero. Hence $E=4\partial_zL$ and

$$
\partial_{\bar z}E=4\partial_{\bar z}\partial_zL=\Delta L=\delta_0.
$$

The analogous [fundamental solution](fundamental-solution-of-a-linear-differential-operator.md) for $\partial_z$ is $1/(\pi\bar z)$. The [singular support](singular-support.md) of each kernel is exactly $\{0\}$: they are smooth elsewhere, and smoothness near zero would make their [Wirtinger derivatives](wirtinger-derivatives.md) smooth there, contradicting the [Dirac delta distribution](dirac-delta-function.md) identity.

```
Target: Distributional Cauchy-Riemann lemma. Parent: Cauchy-Riemann equations. Intended file: analysis.bigb.
```

## ↑ Ancestors (6)

1. [Fundamental solution of a linear differential operator](fundamental-solution-of-a-linear-differential-operator.md)
2. [Distribution theory](distribution-theory-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-distribution-theory-course-of-the-university-of-oxford/2023/3/b/i/solution.md)
