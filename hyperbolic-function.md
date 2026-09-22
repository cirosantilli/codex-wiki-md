# Hyperbolic function

↑ **Parent:** [Exponential function](exponential-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hyperbolic_function)

[Hyperbolic functions](hyperbolic-function.md) combine the [exponential function](exponential-function.md) to describe a [hyperbola](hyperbola.md) much as [trigonometric functions](trigonometric-function.md) describe a [circle](circle.md). Their two basic members are the [hyperbolic cosine](hyperbolic-cosine.md) and [hyperbolic sine](hyperbolic-sine.md), defined for every [real number](real-number.md) $t$ by

$$
\cosh t=\frac{e^t+e^{-t}}2,\qquad \sinh t=\frac{e^t-e^{-t}}2.
$$

Their [derivatives](derivative.md) exchange the two [functions](function-split.md):

$$
\frac{d}{dt}\cosh t=\sinh t,\qquad \frac{d}{dt}\sinh t=\cosh t.
$$

These formulas follow by applying [differentiation](differentiation.md) to the [exponential function](exponential-function.md) definitions. [Gilbert Strang and Edwin Herman, OpenStax Calculus Volume 2, §2.9: hyperbolic definitions and derivatives](https://openstax.org/books/calculus-volume-2/pages/2-9-calculus-of-the-hyperbolic-functions)

Adding and subtracting gives $\cosh t+\sinh t=e^t$ and $\cosh t-\sinh t=e^{-t}$. Multiplying these equalities proves the [hyperbolic Pythagorean identity](hyperbolic-pythagorean-identity.md):

$$
\boxed{\cosh^2t-\sinh^2t=1.}
$$

Consequently the [parametric equation](parametric-equation.md) $(x,y)=(\cosh t,\sinh t)$ traverses the entire right branch of the unit [hyperbola](hyperbola.md) $x^2-y^2=1$, where $x\geq1$. For example, $t=0$ gives $(1,0)$, while $t=\pm1$ gives approximately $(1.543,\pm1.175)$. Compare $(\cos\theta,\sin\theta)$ on the [unit circle](complex-unit-circle.md), where the squared coordinates add to one. The minus sign changes the geometry from a closed [circle](circle.md) to an unbounded [hyperbola](hyperbola.md).

<a id="image-hyperbolic-cosine-and-sine-become-the-coordinates-of-the-right-branch-of-a-unit-hyperbola"></a>
![](hyperbolic-functions-and-unit-hyperbola.png)

**[Figure 16](#image-hyperbolic-cosine-and-sine-become-the-coordinates-of-the-right-branch-of-a-unit-hyperbola). Hyperbolic cosine and sine become the coordinates of the right branch of a unit hyperbola**. The same inputs $t=-1,0,1$ are marked on both [function](function-split.md) graphs and the unit [hyperbola](hyperbola.md). The shaded region has [area](surface-area.md) $1/2$ and corresponds to [hyperbolic angle](hyperbolic-angle.md) $t=1$.

The other members are ratios and reciprocals: [hyperbolic tangent](hyperbolic-tangent.md) is $\tanh t=\sinh t/\cosh t$, [hyperbolic cotangent](hyperbolic-cotangent.md) is $\coth t=\cosh t/\sinh t$, and [hyperbolic secant](hyperbolic-secant.md) is $\operatorname{sech}t=1/\cosh t$; denominators must be nonzero. The [hyperbolic sine](hyperbolic-sine.md) and [hyperbolic cosine](hyperbolic-cosine.md) both solve the [second-order linear differential equation](second-order-linear-differential-equation.md) $f''=f$. In fact $f(t)=A\cosh t+B\sinh t$ has $f(0)=A$ and $f'(0)=B$, making this [basis](basis.md) convenient for an [initial value problem](initial-value-problem.md). Their geometry also makes [hyperbolic substitution](hyperbolic-substitution.md) useful for [integrals](integral.md) containing $\sqrt{1+u^2}$, and the [hyperbolic cosine](hyperbolic-cosine.md) gives the physical [catenary](catenary.md) of a hanging chain.

**Table of contents**

- [Hyperbolic angle](hyperbolic-angle.md)
- [Inverse hyperbolic functions](inverse-hyperbolic-functions.md)
- [Hyperbolic cosine](hyperbolic-cosine.md)
  - [Catenary from hyperbolic cosine](catenary-from-hyperbolic-cosine.md)
  - [Factorial-tail irrationality proof for a hyperbolic cosine](factorial-tail-irrationality-proof-for-a-hyperbolic-cosine.md)
  - [Inverse hyperbolic cosine](inverse-hyperbolic-cosine.md)
- [Hyperbolic sine](hyperbolic-sine.md)
- [Hyperbolic cotangent](hyperbolic-cotangent.md)
  - [Partial-fraction expansion of the hyperbolic cotangent](partial-fraction-expansion-of-the-hyperbolic-cotangent.md)
- [Hyperbolic secant](hyperbolic-secant.md)

## ↑ Ancestors (7)

1. [Exponential function](exponential-function.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Hyperbola](hyperbola.md)
- [Hyperbolic function](hyperbolic-function.md)
- [Hyperbolic Pythagorean identity](hyperbolic-pythagorean-identity.md)
- [Inverse hyperbolic functions](inverse-hyperbolic-functions.md)
- [Partial-fraction expansion of the hyperbolic cotangent](partial-fraction-expansion-of-the-hyperbolic-cotangent.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-2/6d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/8a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-328/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-3/3b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-334/1/e/solution.md)
