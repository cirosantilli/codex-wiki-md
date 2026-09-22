# Machine epsilon

↑ **Parent:** [Floating-point arithmetic](floating-point-arithmetic-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Machine_epsilon)

Here [machine epsilon](machine-epsilon.md) means the gap from one to the next larger value in normalized [floating-point arithmetic](floating-point-arithmetic-split.md):

$$
\epsilon_{\rm mach}=\operatorname{next}(1)-1=\beta^{1-p}.
$$

It is a relative resolution scale near one, not the smallest positive representable value and not a fixed absolute error for all magnitudes. In binary64, $p=53$ gives

$$
\epsilon_{\rm mach}=2^{-52}\approx2.220446049250313\times10^{-16},\qquad u=2^{-53}\approx1.1102230246251565\times10^{-16},
$$

where $u$ is [unit roundoff](unit-roundoff.md) for rounding to nearest. Some authors instead call $u$ their [machine epsilon](machine-epsilon.md); MIT 18.335J uses this half-gap convention. Always check which definition an error bound uses.[Persson, MIT 18.335J, Lecture 2, slides 3, 8–9: the half-gap convention](https://ocw.mit.edu/courses/18-335j-introduction-to-numerical-methods-spring-2019/2f313023ae3404bc217a81a31b227170_MIT18_335JS19_lec2.pdf)

The gap below one is smaller: the preceding binary64 value is $1-2^{-53}$, whereas the next value above one is $1+2^{-52}$. Under nearest-even rounding, `1.0 + 2.0**-53` is exactly `1.0`: the exact [sum](sum.md) is a tie and one has the even final [binary digit](binary-digit.md). By contrast, `1.0 + 2.0**-52` is the next value. Thus searching for the smallest increment that changes one by trial [addition](addition.md) also depends on the rounding convention. At $2^{53}$ the next larger binary64 value is $2^{53}+2$, illustrating why a small absolute increment can disappear at large magnitude.

## ↑ Ancestors (6)

1. [Floating-point arithmetic](floating-point-arithmetic-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Floating-point arithmetic](floating-point-arithmetic-split.md)
- [Machine epsilon](machine-epsilon.md)
- [Round-off error](round-off-error.md)
- [Subnormal number](subnormal-number.md)
