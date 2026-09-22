# First-order unitary product-formula error bound

↑ **Parent:** [Lie product formula](lie-product-formula.md)

For [Hermitian matrices](hermitian-operator.md) $H_1,\ldots,H_m$ and $t\geq0$, let $S(t)=\prod_{j=1}^m e^{-itH_j}$. Then

$$
\boxed{\left\|S(t)-e^{-it\sum_jH_j}\right\|
\leq\frac{t^2}{2}\sum_{j<l}\|[H_j,H_l]\|.}
$$

Here every norm is the [spectral norm](matrix-2-norm.md). A short proof starts with two summands. Differentiate $F(s)=e^{-i(t-s)(A+B)}e^{-isA}e^{-isB}$; its derivative has norm at most $\|[e^{-isA},B]\|$. Differentiating $e^{-iuA}Be^{iuA}$ and integrating yields $\|[e^{-isA},B]\|\leq s\|[A,B]\|$, because [unitary operators](unitary-operator.md) preserve the norm. Integrating $s$ from zero to $t$ gives $t^2\|[A,B]\|/2$. Inductively separate $H_1$ from the remaining sum, use the [triangle inequality](triangle-inequality.md) on their [commutator](commutator.md), and apply the [telescoping bound for products of operators](telescoping-bound-for-products-of-operators.md) to obtain the displayed many-term bound.

Repeating steps of size $t/k$ and telescoping across $k$ steps gives

$$
\left\|S(t/k)^k-e^{-it\sum_jH_j}\right\|
\leq\frac{t^2}{2k}\sum_{j<l}\|[H_j,H_l]\|.
$$

For a chain of $O(n)$ bounded nearest-neighbor terms, only $O(n)$ pairs fail to commute. Consequently first-order [product-formula Hamiltonian simulation](product-formula-hamiltonian-simulation.md) has error $O(nt^2/k)$ and uses $O(nk)$ constant-size gates. The general bound is also given in Proposition 9 of [Childs and collaborators' analysis of Trotter error](https://journals.aps.org/prx/pdf/10.1103/PhysRevX.11.011020).

## ↑ Ancestors (6)

1. [Lie product formula](lie-product-formula.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [First-order two-local Hamiltonian simulation](first-order-two-local-hamiltonian-simulation.md)
- [Lie product formula](lie-product-formula.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/3/a/iii/solution.md)
