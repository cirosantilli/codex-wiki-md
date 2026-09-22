<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Using [functional derivatives](../../../../../../functional-derivative.md) of the interaction functional,

$$
\frac{\delta^2e^{-S_1}}{\delta\widetilde\phi(p)\delta\widetilde\phi(-p)}
=\left[\frac{\delta S_1}{\delta\widetilde\phi(p)}\frac{\delta S_1}{\delta\widetilde\phi(-p)}
-\frac{\delta^2S_1}{\delta\widetilde\phi(p)\delta\widetilde\phi(-p)}\right]e^{-S_1}.
$$

Dividing the flow by $e^{-S_1}$ therefore gives

$$
\boxed{\dot S_1=\frac12\int d^4p\,(2\pi)^4\dot C_\Lambda(p)
\left[\frac{\delta S_1}{\delta\widetilde\phi(p)}\frac{\delta S_1}{\delta\widetilde\phi(-p)}
-\frac{\delta^2S_1}{\delta\widetilde\phi(p)\delta\widetilde\phi(-p)}\right].}
$$

In the first term, remove one leg from each of two interaction vertices and join them with a line weighted by $\dot C_\Lambda(p)$. This produces the tree joining of two vertices. In the second, remove two legs from one vertex and contract them with that line, raising the [loop order](../../../../../../loop-order.md) by one, with [tadpole diagrams](../../../../../../tadpole-diagram.md) as the simplest example. The factor one half accounts for interchanging the contracted ends; the displayed signs are the signs in the interaction-action flow.

**The varying cutoff replaces an internal propagator by its cutoff derivative.** Repeated tree joins and loop closures express how eliminated high-momentum fluctuations generate the vertices of the [Wilsonian effective action](../../../../../../wilsonian-effective-action.md). The action is not restricted to [one-particle-irreducible Feynman diagrams](../../../../../../one-particle-irreducible-feynman-diagram.md): connected tree joins also occur. Field-independent vacuum contributions can again be absorbed into normalization.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
