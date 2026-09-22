<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

For [differentiable maps](../../../../../differentiable-map.md) $F$ at $x$ and $G$ at $F(x)$, the [chain rule](../../../../../chain-rule.md) asserts

$$
D(G\circ F)_x=DG_{F(x)}\circ DF_x.
$$

Write $F(x+h)=F(x)+Ah+r(h)$ with $\|r(h)\|=o(\|h\|)$, and $G(F(x)+u)=G(F(x))+Bu+s(u)$ with $\|s(u)\|=o(\|u\|)$. Since $u=Ah+r(h)=O(\|h\|)$, substitution gives

$$
G(F(x+h))=G(F(x))+BAh+Br(h)+s(Ah+r(h)).
$$

Both remaining terms are $o(\|h\|)$, proving [differentiability](../../../../../differentiability.md) and the stated [chain rule](../../../../../chain-rule.md). The estimate for $s$ also holds when its argument is zero, by setting $s(0)=0$.

For the circle constraint take $H(u)=u_1^2+u_2^2$. The composite $H\circ F$ is constant, so the [chain rule](../../../../../chain-rule.md) gives

$$
0=D(H\circ F)_x=2F(x)^TDF_x.
$$

Since $\|F(x)\|=1$, this is a nonzero row vector annihilating $DF_x$. Thus $DF_x$ cannot be invertible: **$\det DF_x=0$ at every $x$**. Geometrically, the [derivative of a map into a level set](../../../../../derivative-of-a-map-into-a-level-set.md) takes values in the [tangent space](../../../../../tangent-space.md) to the circle.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
