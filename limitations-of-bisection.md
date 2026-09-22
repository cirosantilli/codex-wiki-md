# Limitations of bisection

↑ **Parent:** [Bisection method](bisection-method.md)

Several [zeros of a function](zero-of-a-function.md) can lie in one initial [root bracket](root-bracket.md): the [bisection method](bisection-method.md) seeks one, rather than enumerating them. For instance, the [polynomial](polynomial-split.md) $(x-1)(x-2)(x-3)$ has opposite endpoint signs on $[0,4]$, but its first [midpoint](midpoint.md) evaluation returns only the [polynomial root](root-of-a-polynomial.md) $2$. The initial [zero of a function](zero-of-a-function.md) need not be unique for the [bisection error bound](bisection-error-bound.md) to apply to a retained [zero of a function](zero-of-a-function.md).

A [zero of a function](zero-of-a-function.md) without a sign change cannot be located by the strict sign-change test alone. The [polynomial](polynomial-split.md) $(x-1)^2$ touches zero at $1$ but is positive on either side. On $[0,3]$ both endpoint values are positive: although the [closed interval](closed-real-interval.md) contains a [polynomial root](root-of-a-polynomial.md), it fails the usual starting test for the [bisection method](bisection-method.md). An endpoint or evaluated [midpoint](midpoint.md) [zero of a function](zero-of-a-function.md) can still be recognized directly.

Opposite signs certify a [root bracket](root-bracket.md) only with the required [continuity](continuous-function.md). For $f(x)=1/x$, the values at $-1$ and $1$ have opposite signs, but $f$ is undefined at the [midpoint](midpoint.md) $0$ and has no [zero of a function](zero-of-a-function.md). Hence $[-1,1]$ is invalid input for the [bisection method](bisection-method.md); the [intermediate value theorem](intermediate-value-theorem.md) does not apply across the gap.

## ↑ Ancestors (7)

1. [Bisection method](bisection-method.md)
2. [Bracketing method](bracketing-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Interval bisection](interval-bisection.md)
