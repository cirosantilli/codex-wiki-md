<h1 id="frechet-space">Fréchet space</h1>

↑ **Parent:** [Locally convex space](locally-convex-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fréchet_space)

A Fréchet space is a [Hausdorff](hausdorff-space.md) [locally convex space](locally-convex-space.md) whose [topology](topology-split.md) is induced by a complete translation-invariant [metric](metric.md). Translation invariance means $d(x+z,y+z)=d(x,y)$; [completeness](completeness.md) means every [Cauchy sequence](cauchy-sequence.md) converges in the space. Use a translation-invariant [metric](metric.md) for this condition: an arbitrary compatible [metric](metric.md) can change which [sequences](sequence.md) are [Cauchy sequences](cauchy-sequence.md). [Peter Philip, Functional Analysis, Definition 1.22 and Remark 1.23](https://www.math.lmu.de/~philip/publications/lectureNotes/philipPeter_FunctionalAnalysis.pdf).

Equivalently, the [topology](topology-split.md) comes from a countable [separating family of seminorms](separating-family-of-seminorms.md) $(p_k)_{k\geq0}$ and is complete in their common sense: if $p_k(x_n-x_m)\to0$ as $n,m\to\infty$ for every fixed $k$, then some $x\in E$ satisfies $p_k(x_n-x)\to0$ for every $k$. A useful compatible translation-invariant [metric](metric.md) is

$$
d(x,y)=\sum_{k=0}^{\infty}2^{-(k+1)}\min\{1,p_k(x-y)\}.
$$

It is finite because the weights sum to one. The separating condition makes it a [metric](metric.md); without that condition the formula gives only a [pseudometric](pseudometric.md). Its [convergence in a metric space](convergence-in-a-metric-space.md) and [Cauchy sequence](cauchy-sequence.md) conditions are exactly the conditions for all the $p_k$ separately: control finitely many terms, then bound the remaining tail by $2^{-(K+1)}$. Replacing $p_k$ by $\max_{0\leq j\leq k}p_j$ gives an increasing family with the same [topology](topology-split.md).

Every [Banach space](banach-space-split.md) is a [Fréchet space](frechet-space.md), using its [norm](norm.md) as the single measurement. The [space of smooth functions on a compact interval](space-of-smooth-functions-on-a-compact-interval.md) is a [Fréchet space](frechet-space.md) with [derivative seminorms](derivative-seminorms-on-a-compact-interval.md) but with no single [norm](norm.md) inducing its smooth [topology](topology-split.md). This is why [Fréchet spaces](frechet-space.md) are useful in [differential equations](differential-equation-split.md): one can require accuracy in every order of [derivative](derivative.md), while each particular estimate uses only finitely many orders.

The name honors [Maurice Fréchet](maurice-frechet.md). His doctoral thesis was published as [Sur quelques points du calcul fonctionnel, Rendiconti del Circolo Matematico di Palermo 22, pages 1–72 (1906)](https://link.springer.com/article/10.1007/BF03018603); an [open scan of Fréchet's original paper](https://zenodo.org/records/1428464) is available. This identifies a historical source without attributing the modern locally convex definition to that paper.

**Table of contents**

- [Derivative seminorms on a compact interval](derivative-seminorms-on-a-compact-interval.md)
  - [Smooth convergence on a compact interval](smooth-convergence-on-a-compact-interval.md)

## ↑ Ancestors (7)

1. [Locally convex space](locally-convex-space.md)
2. [Topological vector space](topological-vector-space-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (13)

- [Closed graph theorem for Fréchet spaces](closed-graph-theorem-for-frechet-spaces.md)
- [Fréchet space](frechet-space.md)
- [Open mapping theorem for Fréchet spaces](open-mapping-theorem-for-frechet-spaces.md)
- [Original and weak continuity of linear maps between Fréchet spaces](original-and-weak-continuity-of-linear-maps-between-frechet-spaces.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-5/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-327/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327/1/a/i/solution.md)
- [Sequential continuity criterion in a metrizable vector space](sequential-continuity-criterion-in-a-metrizable-vector-space.md)
- [Space of smooth functions](space-of-smooth-functions.md)
- [Topological vector space](topological-vector-space-split.md)
