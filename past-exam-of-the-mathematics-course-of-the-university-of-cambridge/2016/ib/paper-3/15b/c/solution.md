<h1 id="15b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [wave equation](../../../../../../wave-equation-split.md), introduce characteristic coordinates $\xi=x-ct$, $\eta=x+ct$ when $c\ne0$. The equation becomes $u_{\xi\eta}=0$, so $u=F(x-ct)+G(x+ct)$. The [initial conditions](../../../../../../initial-condition.md) imply $F+G=\phi$ and $-cF'+cG'=0$. Constants can be absorbed into $F,G$, giving the [D'Alembert formula](../../../../../../d-alembert-s-formula.md)

$$
\boxed{u(x,t)=\frac12\bigl[\phi(x-ct)+\phi(x+ct)\bigr].}
$$

If $\phi$ vanishes outside $[-\alpha,\alpha]$, then $u(x,t)=0$ whenever $|x|>\alpha+|c|t$. Thus **Property P fails: the wave equation has [finite propagation speed](../../../../../../finite-propagation-speed.md) $|c|$**. No arbitrarily short time can transmit the disturbance arbitrarily far. If $c=0$, the zero initial velocity instead gives $u(x,t)=\phi(x)$, and the conclusion still holds.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15B](../../15b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
