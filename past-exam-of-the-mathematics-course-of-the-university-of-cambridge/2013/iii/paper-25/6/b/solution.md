<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [Itô product rule](../../../../../../ito-product-rule.md) to the deterministic discount factor and $u(X_t)$:

$$
d(e^{-\lambda t}u(X_t))=e^{-\lambda t}(\mathcal Lu-\lambda u)(X_t)\,dt+e^{-\lambda t}\nabla u(X_t)^{\mathsf T}\sigma(X_t)\,dW_t.
$$

The prescribed differential equation makes the drift vanish. Therefore

$$
\boxed{M_t=e^{-\lambda t}u(X_t)\text{ is a local martingale}.}
$$

This is the discounted generator-eigenfunction martingale underlying the [Feynman-Kac formula](../../../../../../feynman-kac-formula.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
