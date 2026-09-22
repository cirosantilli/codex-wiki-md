<h1 id="6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each $\xi<\kappa$, choose a maximal [antichain in a forcing order](../../../../../../../antichain-in-a-forcing-order.md) below $p$ deciding a witness $\eta>\xi$ in $\dot C$. Write the decided values as $\eta_{\xi,q}$, one for each condition $q$ in that antichain. The $\kappa$-[chain condition for forcing](../../../../../../../chain-condition-for-forcing.md) gives fewer than $\kappa$ possible values. Since $\kappa$ is regular in $M$, choose

$$
g(\xi)=\sup\{\eta_{\xi,q}+1:q\text{ is in the chosen antichain}\}<\kappa.
$$

The [possible-values lemma for chain-condition forcing](../../../../../../../possible-values-lemma-for-chain-condition-forcing.md) ensures

$$
p\Vdash\exists\eta\in\dot C\ (\xi<\eta<g(\xi)).
$$

In $M$ take the [club set](../../../../../../../club-set.md) of limit closure points

$$
\boxed{D=\{\delta<\kappa:\delta\text{ is limit and }
\forall\xi<\delta\ g(\xi)<\delta\}.}
$$

It is unbounded by repeatedly closing any starting ordinal under $g$ for countably many steps, and closed by taking increasing limits. For $\delta\in D$, the forced displayed property gives points of $\dot C$ arbitrarily high below $\delta$. Its forced closedness yields $\delta\in\dot C$. Therefore

$$
\boxed{D\in M\text{ is club},\qquad p\Vdash\check D\subseteq\dot C.}
$$

This proves the [ground-model club containment lemma](../../../../../../../ground-model-club-containment-lemma.md). The name on the right is $\dot C$, as printed in the PDF.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
