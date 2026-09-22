# Support and singular support rules for convolution

↑ **Parent:** [Convolution of distributions with a compactly supported factor](convolution-of-distributions-with-a-compactly-supported-factor.md)

If at least one of $u,v\in\mathcal D'(\mathbb R^n)$ is a [compactly supported distribution](compactly-supported-distribution.md), then

$$
\operatorname{supp}(u*v)\subseteq\operatorname{supp}u+\operatorname{supp}v,\qquad
\operatorname{sing\,supp}(u*v)\subseteq\operatorname{sing\,supp}u+\operatorname{sing\,supp}v.
$$

The sums are [Minkowski sums](minkowski-addition.md). The first rule follows from the pairing $\langle u_x\otimes v_y,\phi(x+y)\rangle$: a [test function](test-function.md) away from the support sum gives zero. For the second rule, localize the output to a small [compact set](compact-space.md) avoiding the sum of the [singular supports](singular-support.md). The relevant pairs of input points form a [compact set](compact-space.md) because one input [support](support.md) is compact. Cover it by finitely many product neighborhoods on each of which at least one input [distribution](distribution-mathematical-analysis.md) is smooth; otherwise the output would meet the sum of the [singular supports](singular-support.md). Smooth cutoffs in these neighborhoods decompose the localized pairing into finitely many [convolutions](convolution.md) with a smooth compactly supported factor. Each is smooth by [smoothing convolution with a test function](smoothing-convolution-with-a-test-function.md). This proves the second rule locally.

The same argument works when addition is a [proper map](proper-map.md) on the product of the two [supports](support.md). Some condition defining the [convolution](convolution.md) is necessary; arbitrary pairs of [distributions](distribution-mathematical-analysis.md) cannot always be convolved.

```
Target: Cauchy kernel fundamental solution. Parent: Fundamental solution of a linear differential operator. Intended file: distribution-theory.bigb.
```

## ↑ Ancestors (7)

1. [Convolution of distributions with a compactly supported factor](convolution-of-distributions-with-a-compactly-supported-factor.md)
2. [Convolution](convolution.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-distribution-theory-course-of-the-university-of-oxford/2023/3/a/iv/solution.md)
- [Solution](past-exam-of-the-distribution-theory-course-of-the-university-of-oxford/2023/3/b/iii/solution.md)
