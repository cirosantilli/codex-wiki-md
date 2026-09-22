<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $N\ge2$, each adjacent pair of walkways has relative [rapidity](../../../../rapidity.md) $\phi_N=\operatorname{artanh}(1/N)$. There are $N$ such steps between $P_0$ and $P_N$, so the [equal-rapidity chain of collinear Lorentz boosts](../../../../equal-rapidity-chain-of-collinear-lorentz-boosts.md) has total [rapidity](../../../../rapidity.md) $N\phi_N$. Thus the actual [velocity](../../../../velocity.md) is

$$
\boxed{v_N=c\tanh\left(N\operatorname{artanh}\frac1N\right)
=c\frac{\left(\frac{N+1}{N-1}\right)^N-1}{\left(\frac{N+1}{N-1}\right)^N+1}.}
$$

It is strictly below the [speed of light](../../../../speed-of-light.md) for every finite $N\ge2$. Adding the adjacent [velocities](../../../../velocity.md) as ordinary numbers ignores the [relativistic velocity-addition formula](../../../../velocity-addition-formula.md).

For large $N$, the [Taylor series](../../../../taylor-series.md) of the inverse [hyperbolic tangent](../../../../hyperbolic-tangent.md) gives

$$
N\operatorname{artanh}(1/N)=1+\frac1{3N^2}+O(N^{-4}).
$$

Consequently

$$
\boxed{v_N\sim c\tanh1=\frac{e^2-1}{e^2+1}\,c\approx0.761594156\,c.}
$$

More precisely, $v_N/c=\tanh1+\operatorname{sech}^2(1)/(3N^2)+O(N^{-4})$, so the limit is approached from above. The case $N=1$ would prescribe an adjacent relative [velocity](../../../../velocity.md) equal to the [speed of light](../../../../speed-of-light.md); it does not define an admissible walkway [inertial frame](../../../../inertial-frame.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
