<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the derivative to transport the planes:

$$
\boxed{\phi_t^*((x,v),L)=\bigl(\phi_t(x,v),D\phi_t(x,v)L\bigr).}
$$

The derivative is an invertible linear map, so it sends a two-dimensional subspace to a two-dimensional subspace. The flow identity $\phi_t\circ\phi_s=\phi_{t+s}$ gives

$$
D\phi_tF(x,v)=F(\phi_t(x,v)).
$$

Hence a plane containing the generator is sent to another plane containing the generator; the displayed formula is a well-defined smooth lift to $\Lambda(SM)$. The [chain rule](../../../../../../chain-rule.md) gives $\phi_{t+s}^*=\phi_t^*\circ\phi_s^*$, and $\phi_0^*$ is the identity. Thus it is a genuine lifted [smooth flow](../../../../../../smooth-flow.md), with inverse $\phi_{-t}^*$, rather than merely a family of maps of individual fibres. Its generator is $F^*=\left.\partial_t\phi_t^*\right|_{t=0}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
