<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define

$$
H(x)=\frac{e^{-x}}{\sqrt x}\qquad(x>0).
$$

This is a [Lebesgue integrable function](../../../../lebesgue-integrable-function.md): on $(0,1]$ it is bounded by $x^{-1/2}$, whose [integral](../../../../integral-split.md) is two, while on $[1,\infty)$ it is bounded by $e^{-x}$, whose [integral](../../../../integral-split.md) is $e^{-1}$. Since $|\sin(xy)|\leq x|y|$,

$$
|h_y(x)|\leq|y|H(x).
$$

Thus **$h_y$ is [Lebesgue integrable](../../../../lebesgue-integrable-function.md) for every $y\geq0$**, including $h_0=0$; the same argument actually works for all real $y$.

The [mean value theorem](../../../../mean-value-theorem.md) for the [sine](../../../../sine.md) gives $|\sin u-\sin v|\leq|u-v|$. Hence

$$
|h_y(x)-h_z(x)|\leq|y-z|H(x)
$$

and the [triangle inequality for an integral](../../../../integral-triangle-inequality.md) gives

$$
\boxed{|F(y)-F(z)|\leq\left(\int_0^\infty H(x)\,dx\right)|y-z|.}
$$

Thus $F$ is a [globally Lipschitz function](../../../../globally-lipschitz-function.md), in particular **continuous on $[0,\infty)$**, including the endpoint zero.

For the [derivative](../../../../derivative.md), fix $y>0$ and take nonzero $t$ sufficiently small that $y+t>0$. The difference quotient has the [integrand](../../../../integrand.md)

$$
D_t(x)=\frac{e^{-x}}{x\sqrt x}\frac{\sin(x(y+t))-\sin(xy)}{t}.
$$

For every $x>0$, $D_t(x)\to H(x)\cos(xy)$ as $t\to0$. The same [mean value theorem](../../../../mean-value-theorem.md) gives the uniform-in-$t$ bound $|D_t(x)|\leq H(x)$.

The [dominated convergence theorem](../../../../dominated-convergence-theorem.md) states that if [measurable functions](../../../../measurable-function.md) $u_n$ converge [almost everywhere](../../../../almost-everywhere.md) to $u$ and $|u_n|\leq G$ for a single [Lebesgue integrable function](../../../../lebesgue-integrable-function.md) $G$, then $u$ is [Lebesgue integrable](../../../../lebesgue-integrable-function.md) and $\int|u_n-u|\to0$, hence $\int u_n\to\int u$. Apply it to the difference quotients along every sequence $t_n\to0$, using the common dominator $H$. The resulting [limit](../../../../limit-of-a-function.md) is independent of the sequence, so

$$
\boxed{F'(y)=\int_0^\infty e^{-x}\frac{\cos(xy)}{\sqrt x}\,dx\qquad(y>0).}
$$

The right-hand [integral](../../../../integral-split.md) is absolutely convergent because its [integrand](../../../../integrand.md) has absolute value at most $H$. This is [dominated differentiation under the integral sign](../../../../dominated-differentiation-under-the-integral-sign.md), justified by an explicit integrable bound rather than a formal interchange.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the integration course of the University of Oxford](../../../split.md)
5. [Integration course of the University of Oxford](../../../../integration-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
