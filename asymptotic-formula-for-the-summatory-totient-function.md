# Asymptotic formula for the summatory totient function

↑ **Parent:** [Summatory totient function](summatory-totient-function.md)

A smoothed form of the [summatory totient function](summatory-totient-function.md) satisfies

$$
\sum_{n\le x}\varphi(n)(x-n)=\frac{x^3}{\pi^2}+O(x^{5/2}).
$$

Use the [Dirichlet series](dirichlet-series.md) $\zeta(s-1)/\zeta(s)$ and the kernel $x^s/[s(s+1)]$ to write the left side as a vertical [contour integral](contour-integral.md). Move the line from real part greater than two to $3/2$. The only crossed pole is at two, with residue $x^3/(6\zeta(2))=x^3/\pi^2$; the remaining vertical integral is $O(x^{5/2})$ by the standard zeta bounds in the half-strip. If $A(x)=\sum_{n\le x}\varphi(n)$ and $S(x)=\int_0^xA(t)\,dt$, positivity of the summands makes $A$ nondecreasing. The backward and forward difference quotients of $S$ bound $A(x)$. Insert $S(x)\sim x^3/\pi^2$, then let the relative difference-quotient step tend to zero, proving the displayed asymptotic. This [monotone integral Tauberian lemma](monotone-integral-tauberian-lemma.md) justifies the passage from a smoothed estimate to an unsmoothed one.

## ↑ Ancestors (6)

1. [Summatory totient function](summatory-totient-function.md)
2. [Euler totient function](euler-totient-function.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
