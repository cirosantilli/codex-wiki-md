# Schauder approximation lemma

↑ **Parent:** [Schauder fixed-point theorem](schauder-fixed-point-theorem.md)

Let $K$ be a nonempty compact [convex set](convex-set-split.md) in a [Banach space](banach-space-split.md) and $T:K\to K$ a [continuous map](continuous-map.md). For every $\varepsilon>0$, there is a finite-dimensional [linear subspace](vector-subspace.md) $L_\varepsilon$ and a [continuous map](continuous-map.md) $T_\varepsilon:K\to K\cap L_\varepsilon$ that approximates $T$ uniformly to within $\varepsilon$ in [norm](norm.md).

Choose $y_1,\ldots,y_N\in T(K)$ whose open radius-$\varepsilon$ [balls](ball-mathematics.md) cover the compact image $T(K)$. Set $w_i(x)=\max\{0,\varepsilon-\|Tx-y_i\|\}$ and

$$
T_\varepsilon(x)=\frac{\sum_iw_i(x)y_i}{\sum_iw_i(x)}.
$$

The denominator is positive. This [convex combination](convex-combination.md) belongs to $K\cap\operatorname{span}\{y_1,\ldots,y_N\}$ and depends continuously on $x$. Every contributing $y_i$ has [distance](distance.md) less than $\varepsilon$ from $Tx$, so the [triangle inequality](triangle-inequality.md) gives $\|T_\varepsilon(x)-Tx\|<\varepsilon$.

## ↑ Ancestors (6)

1. [Schauder fixed-point theorem](schauder-fixed-point-theorem.md)
2. [Fixed-point theorem](fixed-point-theorem.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford/2023/2/a/iii/solution.md)
- [Schauder fixed-point theorem](schauder-fixed-point-theorem.md)
