# Positive-weight expectation cone

↑ **Parent:** [Strictly positive barycentre cone lemma](strictly-positive-barycentre-cone-lemma.md)

For an [integrable](integrability.md) finite-dimensional [random vector](random-vector.md) $Y$, let $L=\{h:h\cdot Y=0\text{ almost surely}\}^\perp$. The displayed [convex cone](convex-cone.md) is open relative to $L$. Given a bounded strictly positive $Z$, the perturbation $Z_\varepsilon=Z(1+\varepsilon\cdot Y/(1+\|Y\|))$, $\|\varepsilon\|<1$, changes its weighted [expectation](expected-value.md) by $A_Z\varepsilon$, where

$$
A_Z=\mathbb E\frac{ZYY^T}{1+\|Y\|}.
$$

For $0\ne v\in L$, $v^TA_Zv>0$: otherwise $v\cdot Y=0$ [almost surely](almost-sure-convergence.md). Thus $A_Z$ is invertible on $L$, and these perturbations give a neighborhood of every point of the cone. The [hyperplane separation theorem](hyperplane-separation-theorem.md) consequently gives the alternative: either zero is a strictly positively weighted [expectation](expected-value.md), or a nonzero direction in $L$ has a nonnegative [dot product](dot-product.md) with $Y$ [almost surely](almost-sure-convergence.md) and a positive [dot product](dot-product.md) with positive [probability](probability.md). To obtain the latter assertion, test the separating direction with $Z=\mathbf1_{\{h\cdot Y<0\}}+\varepsilon$ and let $\varepsilon\downarrow0$.

## ↑ Ancestors (7)

1. [Strictly positive barycentre cone lemma](strictly-positive-barycentre-cone-lemma.md)
2. [Convex cone](convex-cone.md)
3. [Convex set](convex-set.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29/1/solution.md)
- [Positive-density separation proof of the one-period asset-pricing theorem](positive-density-separation-proof-of-the-one-period-asset-pricing-theorem.md)
