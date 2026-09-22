# Opposite-flow fidelity identity for quadratic data

↑ **Parent:** [Quadratic fidelity](quadratic-fidelity.md)

Let $w\in BV\cap L^\infty$ and $g\in BV\cap L^2$ on a bounded domain, $F_g(v)=\tfrac12\|v-g\|_2^2$, and $w_{\pm t}=(1-\theta)w+\theta w\circ\Phi_{\pm t}$ for a smooth compactly supported [local flow](local-flow.md). The displayed formula is exact to an $o(t)$ remainder, and $g$ need not be bounded. Writing $J_t=\det D\Phi_t$, its cross-term identity is

$$
\int g(\delta_tw+\delta_{-t}w)=-\int\delta_tg\,\delta_tw+\int g(1-J_{-t})\delta_{-t}w.
$$

The remainder is $o(t)$ because $1-J_{-t}=O(t)$ and weighted $L^1$ convergence follows from

$$
\int|g||\delta_{-t}w|\le K\|\delta_{-t}w\|_1+2\|w\|_\infty\int_{|g|>K}|g|.
$$

First let $t\to0$, then $K\to\infty$. The mass change of $w^2$ under opposite flows is $O(t^2)\|w\|_2^2$. Combined with the [BV jump-product limit with one bounded factor](bv-jump-product-limit-with-one-bounded-factor.md), this evaluates the jump contribution without a bounded fidelity derivative.

## ↑ Ancestors (10)

1. [Quadratic fidelity](quadratic-fidelity.md)
2. [Total variation denoising](total-variation-denoising.md)
3. [Total variation seminorm on a domain](total-variation-seminorm-on-a-domain.md)
4. [Variational regularization](variational-regularization.md)
5. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
6. [Inverse problem](inverse-problem-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (3)

- [BV jump-product limit with one bounded factor](bv-jump-product-limit-with-one-bounded-factor.md)
- [Jump-amplitude inequality for a bounded ROF minimizer](jump-amplitude-inequality-for-a-bounded-rof-minimizer.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-64/2/iii/solution.md)
