<h1 id="14d/solution">Solution</h1>

↑ **Parent:** [14D](../14d.md)

For parameter-dependent [centre manifold theorem](../../../../../centre-manifold-theorem.md), append $\dot\mu=0$. At $(x,y,\mu)=(0,0,0)$ the [eigenvalues](../../../../../eigenvalue.md) are $0,-1,0$: the $y$ direction is strongly stable and $(x,\mu)$ span the extended centre directions. An [extended centre manifold for a parameter](../../../../../extended-centre-manifold-for-a-parameter.md) is an invariant [graph of a function](../../../../../graph-of-a-function.md) $y=h(x,\mu)$ tangent to $y=0$; nearby trajectories approach its reduced dynamics along stable fibers. The stable [eigenvalue](../../../../../eigenvalue.md) remains separated from zero, so local bifurcation and stability are governed by this reduction. This is the parameter-extension content of the requested stable/centre-manifold discussion.

The [centre-manifold invariance equation](../../../../../centre-manifold-invariance-equation.md) is

$$
h_x(\mu x+xh-x^3)=-h+h^2-x^2.
$$

Reflection symmetry permits an invariant [graph of a function](../../../../../graph-of-a-function.md) with $h(-x,\mu)=h(x,\mu)$ and $h(0,\mu)=0$. At quadratic order the left side vanishes and the right side is $-h-x^2$, giving $h=-x^2+O(|\mu|x^2+x^4)$. More explicitly its first mixed coefficient is $2\mu x^2$, found by equating the $\mu x^2$ terms. The reduced equation is

$$
\boxed{\dot x=\mu x-2x^3+O(|\mu|x^3+x^5).}
$$

Thus the origin is locally asymptotically stable for $\mu<0$, becomes a saddle for $\mu>0$, and creates two stable equilibria $x=\pm\sqrt{\mu/2}+O(\mu^{3/2})$, $y=-\mu/2+O(\mu^2)$. This is a **supercritical [pitchfork bifurcation](../../../../../pitchfork-bifurcation-normal-form.md)**. The exact nearby nonzero branches provide a check: the equilibrium equations give

$$
y=1-\sqrt{1+\mu},\qquad x^2=1+\mu-\sqrt{1+\mu},
$$

which are real and nonzero for small positive $\mu$. The omitted branch $y=1+\sqrt{1+\mu}$ is not near the origin. At $\mu=0$ the leading $-2x^3$ also attracts, although at an algebraic rather than exponential rate.

## ↑ Ancestors (10)

1. [14D](../14d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
