<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Representative [normal forms](../../../../../normal-form-dynamical-systems.md) are $\dot x=\mu+x^2$ for a [saddle-node bifurcation](../../../../../saddle-node-bifurcation.md), $\dot x=\mu x-x^2$ for a [transcritical bifurcation](../../../../../transcritical-bifurcation.md), and $\dot x=\mu x-x^3$ for a supercritical [pitchfork bifurcation](../../../../../pitchfork-bifurcation-normal-form.md). Replacing the last cubic term by $+x^3$ gives the subcritical [pitchfork bifurcation](../../../../../pitchfork-bifurcation-normal-form.md).

Treat $\mu$ as a variable with $\dot\mu=0$. The extended [center manifold](../../../../../center-manifold.md) is tangent to $y=0$, so write $y=h(x,\mu)=Ax^2+Bx\mu+C\mu^2+O((|x|+|\mu|)^3)$. Its invariance equation is $h_x\dot x=\dot y$. At quadratic order this reads

$$
(2Ax+B\mu)\mu=(2-A)x^2-Bx\mu-C\mu^2.
$$

Matching coefficients gives $A=2$, $B=-4$, $C=4$. Substitution into the first equation therefore gives

$$
\boxed{y=2x^2-4x\mu+4\mu^2+O(3),\qquad\dot x=\mu+x^2-4x\mu+4\mu^2+O(3).}
$$

Here $O(3)$ denotes total degree at least three in $(x,\mu)$. With $T=t$, $X=x-2\mu$ and $\widetilde\mu=\mu$, this becomes $dX/dT=\widetilde\mu+X^2+O(3)$. Thus $\alpha=1$, $\beta=2$, $\gamma(\mu)=\mu$, and **the bifurcation is a saddle-node**. For negative parameter, the negative-$X$ branch is stable and the positive-$X$ branch unstable along the [center manifold](../../../../../center-manifold.md); the transverse [eigenvalue](../../../../../eigenvalue.md) is near $-1$.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
