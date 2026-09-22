<h1 id="14/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work on an open domain with $xy>0$ and $x\ne0$, where the displayed square root is real and differentiable. Split $u=v+h$ with $v=\phi(xy)$ and $h=\sqrt{xy}\,\psi(y/x)$. For the first term, the [chain rule](../../../../../chain-rule.md) gives

$$
v_{xx}=y^2\phi''(xy),\qquad v_{yy}=x^2\phi''(xy),
$$

so $x^2v_{xx}-y^2v_{yy}=0$.

For the second term, set $t=y/x$. Its first [partial derivatives](../../../../../partial-derivative.md) are

$$
h_x=\frac{\sqrt{xy}}x\left(\frac12\psi(t)-t\psi'(t)\right),\qquad
h_y=\frac{\sqrt{xy}}y\left(\frac12\psi(t)+t\psi'(t)\right).
$$

They show $xh_x+yh_y=h$, the degree-one case of [Euler theorem for homogeneous functions](../../../../../euler-theorem-for-homogeneous-functions.md). Differentiating that identity with respect to each variable yields

$$
xh_{xx}+yh_{xy}=0,\qquad xh_{xy}+yh_{yy}=0.
$$

The mixed [partial derivatives](../../../../../partial-derivative.md) agree here by the [chain rule](../../../../../chain-rule.md). Multiplying these equations by $x$ and $y$, respectively, proves the [second derivative identity for a degree-one homogeneous function](../../../../../second-derivative-identity-for-a-degree-one-homogeneous-function.md):

$$
x^2h_{xx}=-xyh_{xy}=y^2h_{yy}.
$$

Adding the results for $v$ and $h$ verifies the [partial differential equation](../../../../../partial-differential-equation-split.md)

$$
\boxed{x^2u_{xx}-y^2u_{yy}=0.}
$$

Equivalently, $h(\lambda x,\lambda y)=\lambda h(x,y)$ for positive $\lambda$, so the same proof follows directly from its [homogeneous function](../../../../../homogeneous-function.md) property. The statement is local to a domain where the given expression is defined; it does not require assigning values on $x=0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [14](../../14.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
