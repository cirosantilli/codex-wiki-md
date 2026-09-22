# Explicit midpoint linear multistep method

↑ **Parent:** [Linear multistep method](linear-multistep-method-split.md)

For an [ordinary differential equation](ordinary-differential-equation.md) $y'=\Phi(t,y)$, this [linear multistep method](linear-multistep-method-split.md) uses a centered derivative across the two-step interval $[t_{i-1},t_{i+1}]$, evaluated at its midpoint $t_i$. It requires two starting values, $y_0$ and $y_1$. For a sufficiently smooth exact solution, [Taylor's theorem](taylor-s-theorem.md) gives

$$
y(t+h)-y(t-h)=2hy'(t)+\frac{h^3}{3}y'''(t)+O(h^5).
$$

The unscaled local residual is therefore $O(h^3)$ and the method has order two. Its first characteristic polynomial is $z^2-1$, with the simple roots $1,-1$, so it satisfies the [root condition for a multistep method](root-condition-for-a-multistep-method.md); the second root is a [parasitic amplification root](parasitic-amplification-root.md). This two-step method differs from the one-step [midpoint method](midpoint-method.md) and the [implicit midpoint rule](implicit-midpoint-rule.md).

For the special equation $G'=g(t)$ and $G(a)=0$, an even number $n=2r$ of steps gives $y_n=2h\sum_{j=1}^r g(t_{2j-1})$, independently of the odd-index starting value. It is the [composite midpoint quadrature rule](composite-midpoint-quadrature-rule.md) on $r$ intervals of width $2h$. An odd final index depends on $y_1$, which must be specified separately.

## ↑ Ancestors (6)

1. [Linear multistep method](linear-multistep-method-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Explicit midpoint method](explicit-midpoint-method.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/discrete-mathematics-continuous-mathematics-and-probability/6/d/iii/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/discrete-mathematics-continuous-mathematics-and-probability/6/e/solution.md)
