<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

With total density one, the open [probabilities](../../../../probability.md) for the individual gates are $m=S_{10}+S_{11}$ and $h=S_{01}+S_{11}$. Adding the relevant [master equations](../../../../master-equation.md) cancels transitions of the other gate:

$$
\boxed{\dot m=\alpha(S_{00}+S_{01})-\beta(S_{10}+S_{11})
=\alpha(1-m)-\beta m,}
$$



$$
\boxed{\dot h=\gamma(S_{00}+S_{10})-\delta(S_{01}+S_{11})
=\gamma(1-h)-\delta h.}
$$

These marginal [ordinary differential equations](../../../../ordinary-differential-equation.md) hold even for correlated initial gates. Their product gives $S_{11}$ when the independence assumption in part (c) holds. Solving the [first-order linear differential equations](../../../../first-order-linear-differential-equation.md) from the all-closed initial state gives

$$
m(t)=\frac{\alpha}{\alpha+\beta}\bigl(1-e^{-(\alpha+\beta)t}\bigr),\qquad
h(t)=\frac{\gamma}{\gamma+\delta}\bigl(1-e^{-(\gamma+\delta)t}\bigr).
$$

Put $\lambda=\alpha+\beta=\gamma+\delta>0$. Then

$$
S_{11}(t)=S_{11,\infty}(1-e^{-\lambda t})^2,\qquad
S_{11,\infty}=\frac{\alpha\gamma}{\lambda^2}.
$$

For positive opening rates this increases strictly from zero, so its half-[equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) time is uniquely determined by $(1-e^{-\lambda t})^2=1/2$:

$$
\boxed{t_{1/2}=\frac{-\log(1-2^{-1/2})}{\lambda}
=\frac{\log(2+\sqrt2)}{\lambda}.}
$$

If an opening rate is zero, the all-open [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) density is zero and a nontrivial half-rise time is undefined.

## ↑ Ancestors (12)

1. [E](../e.md)
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
