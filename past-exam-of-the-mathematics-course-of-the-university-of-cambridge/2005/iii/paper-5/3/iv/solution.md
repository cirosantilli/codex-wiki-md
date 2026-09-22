<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $r>0$, define the forward and backward [one-sided interval averaging operators](../../../../../../one-sided-interval-averaging-operator.md)

$$
A_r^+f(x)=\frac1r\int_x^{x+r}f(t)\,dt,\qquad
A_r^-f(x)=\frac1r\int_{x-r}^{x}f(t)\,dt,
$$

and set $A_0^\pm f=f$. Each positive-radius average is bounded in [absolute value](../../../../../../absolute-value.md) by $m_u(f)(x)$. Although $x$ is an endpoint of its averaging interval, enlarge that interval slightly so that $x$ is interior, apply the maximal bound and let the enlargement shrink to zero.

To dominate the limiting identity too without assuming the [differentiation](../../../../../../differentiation.md) result we are proving, use the [sublinear operator](../../../../../../sublinear-operator.md)

$$
S(f)=m_u(f)+|f|.
$$

The maximal estimate and [Chebyshev inequality](../../../../../../chebyshev-inequality.md) imply

$$
\lambda\{S(f)>\alpha\}
\leq\lambda\{m_u(f)>\alpha/2\}
+\lambda\{|f|>\alpha/2\}
\leq\frac8\alpha\|f\|_1.
$$

Thus $S$ has [weak type (1,1)](../../../../../../weak-type-1-1.md) and dominates every $A_r^\pm$, including $r=0$.

Smooth [compactly supported](../../../../../../compact-support.md) functions are dense in $L^1$, obtained by truncating and then smoothing with a [compactly supported](../../../../../../compact-support.md) [approximate identity](../../../../../../approximate-identity.md). For each such [continuous function](../../../../../../continuous-function.md) both averages tend to its value at every point. Applying part (ii) to the two families, and intersecting their full-measure convergence sets, gives $A_r^\pm f(x)\to f(x)$ [almost everywhere](../../../../../../almost-everywhere.md).

The forward [difference quotient](../../../../../../difference-quotient.md) of the primitive is $A_r^+f(x)$, and the backward quotient is $A_r^-f(x)$:

$$
\frac{F(x+r)-F(x)}r=A_r^+f(x),\qquad
\frac{F(x-r)-F(x)}{-r}=A_r^-f(x).
$$

They have the same limit, proving **[differentiability](../../../../../../differentiability.md) [almost everywhere](../../../../../../almost-everywhere.md)**, with the stronger conclusion

$$
\boxed{F'(x)=f(x)\quad\text{almost everywhere}.}
$$

This proves [differentiation of an indefinite Lebesgue integral](../../../../../../differentiation-of-an-indefinite-lebesgue-integral.md) directly from the maximal estimate and density, without assuming $m_u(f)\geq|f|$ as an unproved prerequisite.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
