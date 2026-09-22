<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Lanford contraction proof of the Feigenbaum fixed point](../../../../../../lanford-contraction-proof-of-the-feigenbaum-fixed-point.md) replaces an unstable renormalization operator by a contracting Newton correction. Use a [coefficient Banach space for normalized even maps](../../../../../../coefficient-banach-space-for-normalized-even-maps.md), represented by $p(x)=1-x^2h(x^2)$ with an absolutely summable coefficient [norm](../../../../../../norm.md) on $h$. Its complex domain and a small ball are chosen so that every map is admissible and the renormalization composition is analytic there.

A high-accuracy [polynomial](../../../../../../polynomial-split.md) $p_0$ gives an approximate [fixed point](../../../../../../fixed-point.md). Use a bounded invertible approximate inverse $J$ for $D\mathcal T(p_0)-I$, and define

$$
A(p)=p-J[\mathcal T(p)-p].
$$

Rigorous estimates certify

$$
\varepsilon=\|A(p_0)-p_0\|,\qquad
\sup_{\|p-p_0\|\leq r}\|I-J[D\mathcal T(p)-I]\|\leq\kappa<1,
\qquad\varepsilon\leq(1-\kappa)r.
$$

The finite coefficient computations use [interval arithmetic](../../../../../../interval-arithmetic.md) with controlled rounding; analytic estimates bound the infinite tail. Thus the certification applies to the full function space, rather than merely a truncated [polynomial](../../../../../../polynomial-split.md) system.

Part (b) gives a unique [fixed point](../../../../../../fixed-point.md) of $A$ in the certified ball. Invertibility of $J$ makes it a unique [fixed point](../../../../../../fixed-point.md) $g$ of $\mathcal T$ there. The ball also preserves the quadratic critical maximum and nontrivial shape, excluding the constant formal normalized solution. Consequently **an actual locally unique analytic [Feigenbaum fixed point](../../../../../../feigenbaum-renormalization-fixed-point.md) exists**, with the error bound $\|g-p_0\|\leq\varepsilon/(1-\kappa)$. The numerical approximation locates it; rigorous residual, [derivative](../../../../../../derivative.md) and tail bounds establish its existence and uniqueness. This conclusion is local, not a claim of global uniqueness among all analytic solutions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
