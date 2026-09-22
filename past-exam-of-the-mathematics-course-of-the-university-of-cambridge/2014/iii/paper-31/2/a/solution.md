<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Consider the secant slope

$$
H(r)=\frac{M(r)-1}{r},\qquad 0<r<r_\infty.
$$

The [moment-generating function](../../../../../../moment-generating-function.md) is continuous on the interior of its finite domain and has right derivative $M'(0)=\mu$. Thus $H(r)\to\mu$ as $r\downarrow0$. For every fixed positive claim amount $x$, the function $(e^{rx}-1)/r$ is strictly increasing in $r>0$: its derivative has numerator $e^{rx}(rx-1)+1>0$, since this numerator starts at zero and has derivative $rx e^{rx}$ as a function of $rx$. Taking [expected values](../../../../../../expected-value.md) preserves the strict inequality. Therefore $H$ is continuous and strictly increasing. Equivalently, the [strictly convex](../../../../../../strictly-convex-function.md) transform $M$ has strictly increasing secant slopes from the origin.

If $r_\infty<\infty$, the assumed blow-up of $M$ gives $H(r)\to\infty$. If $r_\infty=\infty$, choose $a>0$ with $d=\mathbb P(X_1\ge a)>0$. Such an $a$ exists because the claims are positive. Then $M(r)\ge de^{ar}$, so again $H(r)\to\infty$. This exponential lower bound is needed at an infinite endpoint: mere divergence of $M$ would not, by itself, establish divergence of $M(r)/r$.

The target $(1+\theta)\mu$ strictly exceeds the limiting slope $\mu$. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) and strict monotonicity therefore give

$$
\boxed{\exists!\ R\in(0,r_\infty):\ H(R)=(1+\theta)\mu.}
$$

Multiplying by $R$ gives the defining [adjustment coefficient](../../../../../../adjustment-coefficient.md) equation. The zero root of the undivided equation is excluded. This is the [secant-slope existence criterion for an adjustment coefficient](../../../../../../secant-slope-existence-criterion-for-an-adjustment-coefficient.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
