# Total differential

↑ **Parent:** [Partial derivative](partial-derivative.md)

The [total differential](total-differential.md) is the [linear map](linear-map.md) that combines the first-order responses to simultaneous changes in all coordinates. For a [differentiable](differentiable-function.md) real-valued [function](function-split.md) at $a$, it can be written

$$
df_a(h)=\sum_{j=1}^n\partial_j f(a)\,h_j
=\nabla f(a)\cdot h,\qquad
df=\sum_{j=1}^n\frac{\partial f}{\partial x_j}\,dx_j.
$$

Here $h$ is an input [vector](vector.md); $dx_j$ denotes the coordinate [linear functional](linear-functional.md) $h\mapsto h_j$. The coordinate formula and the [Fréchet derivative](frechet-derivative.md) describe the same [linear map](linear-map.md). The defining approximation is

$$
f(a+h)-f(a)=df_a(h)+o(\|h\|)\qquad(h\to0).
$$

The [little o notation](little-o-notation.md) says the remaining [approximation error](approximation-error.md) becomes small relative to the input [norm](norm.md), across every direction of approach.[Calculus Volume 3, §4.4, differentiability definition (4.26) and total differential (4.27)](calculus-volume-3-by-gilbert-strang-and-others/4-4-tangent-planes-and-linear-approximations.md)

For $f=x^2+xy+2y^2$ at $a=(1,1)$, **$df_a(h,k)=3h+5k$**. A simultaneous change $(h,k)=(0.02,-0.01)$ gives the [linear approximation](linear-approximation.md)

$$
\Delta f\approx3(0.02)+5(-0.01)=\boxed{0.01}.
$$

The exact algebra is

$$
f(1+h,1+k)-4=3h+5k+h^2+hk+2k^2.
$$

Consequently the exact change is $0.0104$, and the [approximation error](approximation-error.md) is $0.0004$. If both input changes are halved, the linear prediction becomes $0.005$ and the error becomes $0.0001$: the first-order response halves, while the quadratic error falls by a factor of four. The right panel under [directional derivative](directional-derivative.md) displays this comparison as the displacement is scaled.

For a quick check of [differentiability](differentiability.md), $|hk|\leq(h^2+k^2)/2$ gives

$$
|h^2+hk+2k^2|\leq\frac52(h^2+k^2).
$$

Dividing by $\sqrt{h^2+k^2}$ makes this bound tend to zero. The same calculation proves that the [tangent plane](tangent-plane.md) to the [graph of a function](graph-of-a-function.md) at $(1,1,4)$ is $z=4+3(x-1)+5(y-1)$. It approximates the entire local surface, rather than only two coordinate slices.

The [total differential](total-differential.md) is useful for estimating the combined effect of small input changes without reevaluating a complicated [function](function-split.md). For example, if $|h|\leq0.02$ and $|k|\leq0.01$, then $|df_a(h,k)|\leq0.11$. The exact remainder bound from the displayed [polynomial](polynomial-split.md) is at most $0.0008$, so this example has $|\Delta f|\leq0.1108$ throughout that input [rectangle](rectangle.md). These are deterministic bounds; a [variance](variance-split.md) calculation additionally needs a [joint probability distribution](joint-probability-distribution.md) and its [covariances](covariance.md). A first-order estimate is also local: large changes require control of the remainder, not merely knowledge of the [partial derivatives](partial-derivative.md) at one point.

## ↑ Ancestors (8)

1. [Partial derivative](partial-derivative.md)
2. [Multivariable calculus](multivariable-calculus-split.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Direct product of integrable Hamiltonian systems](direct-product-of-integrable-hamiltonian-systems.md)
- [Directional derivative](directional-derivative.md)
- [Partial derivative](partial-derivative.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/32c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-3/9a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2/10/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-2/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2005/paper-2/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2009/paper-1/18/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/17/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-1/12/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/12/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2019/paper-1/14/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/14/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1/14/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/14/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/14/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2004/paper-1/1/solution.md)
- [Total differential](total-differential.md)
