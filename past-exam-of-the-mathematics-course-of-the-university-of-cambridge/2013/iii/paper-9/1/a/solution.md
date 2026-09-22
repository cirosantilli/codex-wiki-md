<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a unit direction $e$, let $T_\delta(a,e)$ be a length-one [Kakeya tube](../../../../../../kakeya-tube.md) with transverse radius $\delta$, centered at $a$, and define the [Kakeya maximal function](../../../../../../kakeya-maximal-function.md) by

$$
\mathcal K_\delta f(e)=\sup_a\frac1{|T_\delta(a,e)|}\int_{T_\delta(a,e)}|f(x)|\,dx.
$$

Using normalized surface measure on the direction sphere, the [Kakeya maximal conjecture](../../../../../../kakeya-maximal-conjecture.md) is the following family of estimates, in the formulation relevant to this paper:

$$
\boxed{\|\mathcal K_\delta f\|_{L^n(S^{n-1})}
\le C_{n,\varepsilon}\delta^{-\varepsilon}\|f\|_{L^n(\mathbb R^n)}
\quad(0<\delta<1,\ \varepsilon>0).}
$$

The constant is independent of $\delta$ and $f$. Replacing round [Kakeya tubes](../../../../../../kakeya-tube.md) by comparable rectangular tubes changes only dimensional constants.

A bounded [Kakeya set](../../../../../../kakeya-set.md) contains a unit line segment in every direction. The [Kakeya Minkowski dimension conjecture](../../../../../../kakeya-minkowski-dimension-conjecture.md) says that every such set has full [Minkowski dimension](../../../../../../box-counting-dimension.md) $n$. The maximal estimate in fact gives full lower as well as upper [Minkowski dimension](../../../../../../box-counting-dimension.md).

To prove that implication, let $E_\delta=\{x:\operatorname{dist}(x,E)<\delta\}$. Each unit segment in $E$ has a thinner tube contained in $E_\delta$, so $\mathcal K_{c\delta}\mathbf1_{E_\delta}(e)\ge1$ for every $e$, with a fixed dimensional $c>0$. Apply the maximal estimate to this [indicator function](../../../../../../indicator-function.md):

$$
1\lesssim C_{n,\varepsilon}\delta^{-\varepsilon}|E_\delta|^{1/n},
\qquad |E_\delta|\gtrsim_{n,\varepsilon}\delta^{n\varepsilon}.
$$

If $N_\delta(E)$ is the smallest number of radius-$\delta$ balls covering $E$, that cover, enlarged by a fixed factor, covers $E_\delta$. Thus $|E_\delta|\lesssim_n\delta^n N_\delta(E)$ and

$$
N_\delta(E)\gtrsim_{n,\varepsilon}\delta^{-n+n\varepsilon}.
$$

Taking the lower limit of $\log N_\delta(E)/\log(1/\delta)$ and then letting $\varepsilon\downarrow0$ gives lower [Minkowski dimension](../../../../../../box-counting-dimension.md) at least $n$. Bounded subsets of $\mathbb R^n$ have upper [Minkowski dimension](../../../../../../box-counting-dimension.md) at most $n$. Consequently **both dimensions equal $n$**, which proves the requested implication.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
