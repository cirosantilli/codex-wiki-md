<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\eta=x/y^\beta$ the [chain rule](../../../../../chain-rule.md) gives $u_y=-\beta\eta f'/y$, $u_x=y^{-\beta}f'$ and $(uu_x)_x=y^{-2\beta}[ff''+(f')^2]$. Multiplication of the equation by $y$ gives

$$
-\beta\eta f'=y^{1-2\beta}[ff''+(f')^2]+\tfrac12f.
$$

A nontrivial scale-invariant balance therefore selects $\boxed{\beta=1/2}$ and yields

$$
ff''+(f')^2+\tfrac12\eta f'+\tfrac12f=0.
$$

Its left side is the [derivative](../../../../../derivative.md) of $ff'+\eta f/2$. The [boundary conditions](../../../../../boundary-condition.md) give $f(0)=1$ and $f'(0)=0$, so the integration constant is zero:

$$
f(f'+\eta/2)=0.
$$

On the positive branch before the first zero, divide by $f$ and integrate, obtaining $f=1-\eta^2/4$. Its first positive zero is $\eta_F=2$. Hence

$$
\boxed{u(x,y)=1-\frac{x^2}{4y}\quad(0\leq x\leq2\sqrt y),\qquad x_F(y)=2\sqrt y.}
$$

A direct check gives $u_y=x^2/(4y^2)$ and $(uu_x)_x+u/(2y)=x^2/(4y^2)$. The zero extension past this front is also a natural weak compact-support continuation: $u$ is continuous and the degenerate diffusive [flux](../../../../../flux.md) $uu_x$ tends to zero at the front. This is a [source-driven porous-medium similarity front](../../../../../source-driven-porous-medium-similarity-front.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
