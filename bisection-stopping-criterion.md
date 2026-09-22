# Bisection stopping criterion

↑ **Parent:** [Bisection method](bisection-method.md)

For a requested absolute tolerance $\varepsilon>0$, stop when the retained [root bracket](root-bracket.md) has width at most $2\varepsilon$, and report its [midpoint](midpoint.md). The [bisection error bound](bisection-error-bound.md) then guarantees $|m_k-x_*|\leq\varepsilon$ in exact arithmetic. Using the [ceiling function](ceiling-function.md) and the base-two [logarithm](logarithm.md), the required number of halvings is

$$
k_{\min}=\max\left\{0,\left\lceil\log_2\frac{b-a}{2\varepsilon}\right\rceil\right\}.
$$

The zero allows stopping before any update when the initial [root bracket](root-bracket.md) is already sufficiently narrow. For the [polynomial](polynomial-split.md) $f(x)=x^2-2$ on $[1,2]$ with $\varepsilon=10^{-3}$, $k_{\min}=\lceil\log_2 500\rceil=9$. After nine halvings,

$$
[a_9,b_9]=[1.4140625,1.416015625],\qquad m_9=1.4150390625,\qquad \frac{W_9}{2}=\frac{1}{1024}=0.0009765625.
$$

Thus the reported [midpoint](midpoint.md) meets the tolerance; its actual error from the [square root](square-root.md) $\sqrt2$ is approximately $0.000825500126905$. After eight halvings the bound is $1/512>10^{-3}$, so eight do not give this worst-case guarantee.

Cache the endpoint values. Each update of the [bisection method](bisection-method.md) needs just one new [function](function-split.md) evaluation, at the old [midpoint](midpoint.md). With no early [zero of a function](zero-of-a-function.md), $k$ updates therefore cost $k+2$ [function](function-split.md) evaluations, including the two initial endpoints. Returning the new [midpoint](midpoint.md) requires no additional [function](function-split.md) evaluation; requesting its value would add one. The nine-update example needs eleven evaluations for the guarantee.

A small [function](function-split.md) value $|f(m_k)|$ alone does not guarantee a small position error: rescaling $f$ changes those values without changing its [zeros of a function](zero-of-a-function.md). In a practical implementation, use an explicit width test and an iteration limit. With [floating-point arithmetic](floating-point-arithmetic.md), also stop if the computed [midpoint](midpoint.md) equals either endpoint: the [root bracket](root-bracket.md) can no longer shrink, so repeating the update would loop forever. Report this precision limit separately if the requested tolerance remains unmet. Reliable sign evaluations are needed to preserve the [root bracket](root-bracket.md); compare signs directly rather than multiplying endpoint values, which can suffer overflow or underflow in [floating-point arithmetic](floating-point-arithmetic.md).

For a rounded [midpoint](midpoint.md) $m$ still inside a valid [root bracket](root-bracket.md), the geometric error bound is $\max\{m-a_k,b_k-m\}$; it need not equal $W_k/2$ because of [roundoff error](round-off-error.md). A rigorous computed enclosure also needs conservative arithmetic for that bound and reliable endpoint signs. The exact-arithmetic [bisection error bound](bisection-error-bound.md) should not be claimed unchanged after precision prevents further halving.

For practical tolerance conventions, SciPy's `bisect` combines absolute and relative tolerances through $|x-x_0|\leq\mathrm{xtol}+\mathrm{rtol}|x_0|$, and provides a maximum iteration count and convergence status. These differ from the purely absolute width test above.[SciPy, scipy.optimize.bisect documentation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.bisect.html)

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
