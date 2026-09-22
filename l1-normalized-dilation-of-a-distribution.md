# L1-normalized dilation of a distribution

↑ **Parent:** [Dilation of a distribution](dilation-of-a-distribution.md)

For $\varepsilon>0$ and $u\in\mathcal D'(\mathbb R^n)$, define $u_\varepsilon$ by the displayed pairing. If $u$ is a [regular distribution](regular-distribution.md), this agrees with $u_\varepsilon(x)=\varepsilon^{-n}u(x/\varepsilon)$ and preserves its [L1 space](l1-space.md) norm. With the convention $\delta_tu(x)=u(tx)$ for [dilation of a distribution](dilation-of-a-distribution.md), it equals $\varepsilon^{-n}\delta_{1/\varepsilon}u$.

If $u\in L^1(\mathbb R^n)$, the [dominated convergence theorem](dominated-convergence-theorem.md) gives

$$
\langle u_\varepsilon,\phi\rangle=\int u(y)\phi(\varepsilon y)\,dy
\longrightarrow\phi(0)\int u,
\qquad u_\varepsilon\to\left(\int u\right)\delta_0.
$$

The constant [distribution](distribution-mathematical-analysis.md) $u=1$ instead gives $u_\varepsilon=\varepsilon^{-n}$ and has no limit in [weak convergence of distributions](weak-convergence-of-distributions.md).

```
Target: Restriction of a distribution. Parent: Distribution (mathematical analysis). Intended file: distribution-theory.bigb.
```

## ↑ Ancestors (6)

1. [Dilation of a distribution](dilation-of-a-distribution.md)
2. [Distribution theory](distribution-theory-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-distribution-theory-course-of-the-university-of-oxford/2023/2/a/iii/solution.md)
