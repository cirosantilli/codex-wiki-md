<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The two identical $M$ gates are independent [Bernoulli random variables](../../../../bernoulli-distribution.md), so their open count has a [binomial distribution](../../../../binomial-distribution.md). Multiplying by the independent $H$ factor gives the normalized channel densities

$$
\boxed{S_{ij}=\binom2i m^i(1-m)^{2-i}h^j(1-h)^{1-j}.}
$$

Explicitly,

$$
\begin{aligned}
S_{00}&=(1-m)^2(1-h),&S_{01}&=(1-m)^2h,\\
S_{10}&=2m(1-m)(1-h),&S_{11}&=2m(1-m)h,\\
S_{20}&=m^2(1-h),&S_{21}&=m^2h.
\end{aligned}
$$

The [binomial coefficient](../../../../binomial-coefficient-split.md) $\binom21=2$ counts which of the two distinguishable $M$ gates is open. At open count $i$, the total $M$-opening rate is $(2-i)\alpha$ and the total closing rate is $i\beta$. Dividing the [expected value](../../../../expected-value-split.md) of that count by two therefore recovers the same single-gate [ordinary differential equation](../../../../ordinary-differential-equation.md):

$$
\boxed{\dot m=\alpha(1-m)-\beta m,\qquad
\dot h=\gamma(1-h)-\delta h.}
$$

For the specified [initial conditions](../../../../initial-condition.md) and common rate sum $\lambda$, the all-open fraction is

$$
S_{21}(t)=\frac{\alpha^2\gamma}{\lambda^3}(1-e^{-\lambda t})^3.
$$

Thus, assuming positive opening rates,

$$
\boxed{t_{1/2}=\frac{-\log(1-2^{-1/3})}{\lambda}.}
$$

Three gates take longer to reach half their final all-open fraction than two gates: all three activation factors must build up simultaneously.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
