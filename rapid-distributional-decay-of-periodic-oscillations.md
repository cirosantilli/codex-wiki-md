# Rapid distributional decay of periodic oscillations

↑ **Parent:** [Weak convergence of distributions](weak-convergence-of-distributions.md)

If $f\in L^1(0,1)$ has mean zero, $j$ is a positive integer, and $\phi\in\mathcal D(0,1)$, the displayed estimate holds for every integer $N\geq1$. Let $h_N=P^Nf$ use [periodic primitives with zero mean](periodic-primitive-with-zero-mean.md). Repeated [integration by parts](integration-by-parts.md) gives

$$
\int_0^1\overline f(jx)\phi(x)\,dx
=j^{-N}\int_0^1\overline h_N(jx)\phi^{(N)}(x)\,dx.
$$

There are no [boundary terms](boundary-term.md), and integration over exactly $j$ periods gives $\|\overline h_N(j\,\cdot)\|_{L^1(0,1)}=\|h_N\|_{L^1}\leq\|f\|_{L^1}$. This proves the estimate. In particular, if zero-mean $g_j$ satisfy $\|g_j\|_{L^1}=O(j^m)$, their [periodic extensions](periodic-extension.md) satisfy $\overline g_j(j\,\cdot)\to0$ in [weak convergence of distributions](weak-convergence-of-distributions.md) by choosing $N=m+1$.

```
Target: Essential closure. Parent: Lebesgue measure. Intended file: measure-theory.bigb.
```

## ↑ Ancestors (7)

1. [Weak convergence of distributions](weak-convergence-of-distributions.md)
2. [Distribution (mathematical analysis)](distribution-mathematical-analysis.md)
3. [Distribution theory](distribution-theory-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-distribution-theory-course-of-the-university-of-oxford/2023/2/b/iii/solution.md)
