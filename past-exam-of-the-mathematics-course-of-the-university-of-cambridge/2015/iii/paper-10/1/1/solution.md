<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For the [wave equation](../../../../../../wave-equation-split.md) with [d'Alembert operator](../../../../../../d-alembert-operator.md) $\Box=-\partial_t^2+\Delta$, the [wave speed](../../../../../../wave-speed.md) is one. **The [domain of dependence](../../../../../../domain-of-dependence.md) of $(t,x)$ is the initial ball $\overline B(x,t)$.** More precisely, two solutions whose [Cauchy data](../../../../../../cauchy-data.md) agree on a neighbourhood of that ball have the same value at $(t,x)$. Thus, if both [Cauchy data](../../../../../../cauchy-data.md) have [support](../../../../../../support.md) in $K$, [finite propagation speed](../../../../../../finite-propagation-speed.md) gives

$$
\operatorname{supp}\phi(t,\cdot)\subseteq\{x:\operatorname{dist}(x,K)\leq t\},\qquad t\geq0.
$$

The [Strong Huygens principle](../../../../../../strong-huygens-principle.md) is sharper in three spatial dimensions: **only the initial data on the sphere $|y-x|=t$ contribute**, including the first spatial derivatives of the initial displacement there. The [Kirchhoff formula](../../../../../../kirchhoff-formula.md) makes this precise:

$$
\phi(t,x)=\partial_t\left(\frac{t}{4\pi}\int_{S^2}\phi_0(x+t\omega)\,d\omega\right)
+\frac{t}{4\pi}\int_{S^2}\phi_1(x+t\omega)\,d\omega.
$$

In particular, if the [Cauchy data](../../../../../../cauchy-data.md) have [compact support](../../../../../../compact-support.md) in $\overline B(0,R)$, then

$$
\boxed{\phi(t,x)=0\quad\text{whenever}\quad \bigl||x|-t\bigr|>R.}
$$

For $t>R$, the solution therefore vanishes behind the inward edge $|x|=t-R$ as well as outside $|x|=t+R$. The absence of an interior tail is the additional content of the [Strong Huygens principle](../../../../../../strong-huygens-principle.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
