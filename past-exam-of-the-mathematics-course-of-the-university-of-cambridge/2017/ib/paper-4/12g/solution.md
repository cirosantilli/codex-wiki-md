<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

A function $f:U\to\mathbb R^n$ has a [Fréchet derivative](../../../../../frechet-derivative.md) at $a\in U$ if there is a [linear map](../../../../../linear-map.md) $A:\mathbb R^m\to\mathbb R^n$ such that

$$
\boxed{f(a+h)=f(a)+Ah+o(\|h\|)\quad(h\to0)}.
$$

The remainder condition is a limit in all directions at once, not merely the existence of [partial derivatives](../../../../../partial-derivative.md).

For the stated scalar two-variable result, fix $a=(a_1,a_2)$ and choose a small rectangle contained in the open set $U$. Split the increment into two coordinate segments. Applying the one-dimensional [mean value theorem](../../../../../mean-value-theorem.md) on each segment yields

$$
f(a_1+h,a_2+k)-f(a)
=h f_x(a_1+\theta h,a_2+k)+k f_y(a_1,a_2+\sigma k)
$$

for $\theta,\sigma\in(0,1)$, omitting a term if its increment is zero. Subtract $h f_x(a)+k f_y(a)$. By [continuity](../../../../../continuous-function.md) of the [partial derivatives](../../../../../partial-derivative.md), for any $\varepsilon>0$ the remainder has modulus at most $\varepsilon(|h|+|k|)\leq\sqrt2\varepsilon\sqrt{h^2+k^2}$ for sufficiently small increments. This proves [differentiability](../../../../../differentiability.md), with [Jacobian matrix](../../../../../jacobian-matrix.md) $(f_x(a),f_y(a))$.

Away from the origin the specified [rational function](../../../../../rational-function.md) has a nonzero denominator and is [smooth](../../../../../smooth-function.md). At the origin, $f(t,0)=t$ and $f(0,t)=2t^2$, so the [partial derivatives](../../../../../partial-derivative.md) are $f_x(0,0)=1$, $f_y(0,0)=0$. Any [Fréchet derivative](../../../../../frechet-derivative.md) there would therefore be $A(h,k)=h$. However,

$$
f(t,t)=\frac t2+t^2,\qquad
\frac{|f(t,t)-t|}{\sqrt2|t|}\longrightarrow\frac1{2\sqrt2}\ne0.
$$

Thus

$$
\boxed{f\text{ is differentiable exactly on }\mathbb R^2\setminus\{(0,0)\}}.
$$

The failure is not merely a failure of [continuity](../../../../../continuous-function.md): $|f(x,y)|\leq |x|+2y^2\to0$ at the origin, so the function is [continuous](../../../../../continuous-function.md) there.

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
