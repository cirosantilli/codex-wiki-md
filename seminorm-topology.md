# Seminorm topology

↑ **Parent:** [Locally convex space](locally-convex-space.md)

Given a nonempty family $\mathcal P$ of finite-valued [seminorms](seminorm.md) on a real or complex [vector space](vector-space-split.md) $E$, its seminorm topology has basic open zero [neighbourhoods](neighbourhood-mathematics.md)

$$
U(p_1,\ldots,p_m;\varepsilon_1,\ldots,\varepsilon_m)
=\bigcap_{i=1}^m\{x\in E:p_i(x)<\varepsilon_i\},
\qquad p_i\in\mathcal P,\quad\varepsilon_i>0.
$$

Their translates form a [basis of a topology](basis-of-a-topology.md). Only finite [intersections](set-intersection.md) are required: an infinite [intersection](set-intersection.md) might impose a stronger [topology](topology-split.md). Equivalently, put $q(x)=\max_i p_i(x)/\varepsilon_i$; then $q$ is a [seminorm](seminorm.md) and $U=\{q<1\}$. See [Günther Hörmann, Advanced Functional Analysis, section 4, neighbourhood systems from seminorms](https://www.mat.univie.ac.at/~gue/lehre/25AFA/AFA.pdf) for the general construction.

Each defining [seminorm](seminorm.md) is [continuous](continuous-function.md), since $|p(x)-p(y)|\leq p(x-y)$. A [sequence](sequence.md) satisfies $x_n\to x$ precisely when $p(x_n-x)\to0$ for every $p\in\mathcal P$; the same criterion holds for [nets](net-mathematics.md). Finitely many measurements can each meet a prescribed tolerance after a common index.

The [seminorm](seminorm.md) axioms also establish the required joint [continuity](continuous-function.md) of [vector addition](vector-addition.md) and [scalar multiplication](scalar-multiplication.md):

$$
p\bigl((x+y)-(x_0+y_0)\bigr)\leq p(x-x_0)+p(y-y_0),
\qquad
p(\lambda x-\lambda_0x_0)\leq |\lambda|p(x-x_0)+|\lambda-\lambda_0|p(x_0).
$$

For a basic [neighbourhood](neighbourhood-mathematics.md), apply these estimates to its finitely many [seminorms](seminorm.md); near $\lambda_0$ the [absolute value](absolute-value.md) $|\lambda|$ is bounded. This gives a [locally convex space](locally-convex-space.md) even when some directions are invisible to every measurement.

**Table of contents**

- [Separating family of seminorms](separating-family-of-seminorms.md)

## ↑ Ancestors (7)

1. [Locally convex space](locally-convex-space.md)
2. [Topological vector space](topological-vector-space-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Derivative seminorms on a compact interval](derivative-seminorms-on-a-compact-interval.md)
- [Locally convex space](locally-convex-space.md)
- [Seminorm](seminorm.md)
- [Separating family of seminorms](separating-family-of-seminorms.md)
- [Topological vector space](topological-vector-space-split.md)
