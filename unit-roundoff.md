# Unit roundoff

↑ **Parent:** [Floating-point arithmetic](floating-point-arithmetic-split.md)

For [floating-point arithmetic](floating-point-arithmetic-split.md) with precision $p$ in radix $\beta$ and rounding to nearest, [unit roundoff](unit-roundoff.md) is the half-gap scale $u=\beta^{1-p}/2$. If a nonzero exact [real number](real-number.md) $z$ lies in the normal finite range, its nearest rounded value satisfies

$$
\operatorname{fl}(z)=z(1+\delta),\qquad |\delta|\leq u.
$$

Indeed, the absolute distance to the nearest value is at most $\Delta_e/2$, and $|z|\geq\beta^e$ gives the bound. For a correctly rounded [addition](addition.md), [subtraction](subtraction.md), [multiplication](multiplication.md) or [division](division-mathematics.md), apply this estimate to the exact result of that one operation on the stored operands. The bound does not include earlier [roundoff error](round-off-error.md) or automatically bound a whole [algorithm](algorithm-split.md). Results outside the finite range and tiny [subnormal numbers](subnormal-number.md) require separate treatment. Rounding in a directed mode also changes the bound.[Goldberg, 1991, §§Relative Error and Ulps, Exactly Rounded Operations](https://docs.oracle.com/cd/E19957-01/806-3568/ncg_goldberg.html)

## ↑ Ancestors (6)

1. [Floating-point arithmetic](floating-point-arithmetic-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Catastrophic cancellation](catastrophic-cancellation.md)
- [Floating-point arithmetic](floating-point-arithmetic-split.md)
- [Machine epsilon](machine-epsilon.md)
- [Subnormal number](subnormal-number.md)
- [Unit roundoff](unit-roundoff.md)
