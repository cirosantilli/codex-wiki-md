# Root sensitivity in power-sum reconstruction

↑ **Parent:** [Newton's identities](newton-s-identities.md)

Exact reconstruction does not promise that small errors in [power sums](power-sum-symmetric-polynomial.md) produce proportionally small errors in individual [polynomial roots](root-of-a-polynomial.md). For two roots, let $p_1=2$ and $p_2=2+\delta$. [Newton's identities](newton-s-identities.md) give $e_1=2$ and $e_2=1-\delta/2$, so the [monic polynomial](monic-polynomial.md) is $(z-1)^2-\delta/2$. Its [polynomial roots](root-of-a-polynomial.md) are $1\pm\sqrt{\delta/2}$. A zero value of $\delta$ gives a [multiple root](multiple-root.md); positive $\delta$ splits it into two real roots, and negative $\delta$ splits it into a complex-conjugate pair.

With $\delta=2\varepsilon^2>0$, the second [power sum](power-sum-symmetric-polynomial.md) changes by $2\varepsilon^2$ while each [polynomial root](root-of-a-polynomial.md) moves by $\varepsilon$. The ratio $1/(2\varepsilon)$ grows without bound as $\varepsilon$ tends to zero. Thus [coefficients](coefficient.md) can stay close while individual root locations are more sensitive. This is a reason to distinguish recovering [coefficients](coefficient.md) by [Newton's identities](newton-s-identities.md) from subsequently approximating the [polynomial roots](root-of-a-polynomial.md).

## ↑ Ancestors (7)

1. [Newton's identities](newton-s-identities.md)
2. [Elementary symmetric polynomial](elementary-symmetric-polynomial.md)
3. [Polynomial](polynomial-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
