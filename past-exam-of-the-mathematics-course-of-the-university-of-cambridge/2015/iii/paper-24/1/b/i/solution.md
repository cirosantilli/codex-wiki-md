<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [order completeness](../../../../../../../order-completeness.md) of $\mathbb R$ to define

$$
\boxed{\widetilde\varphi(x)=\sup\{\varphi(d):d\in D, d<x\}.}
$$

The set in this [supremum](../../../../../../../supremum.md) is nonempty and bounded above: choose $d_0,d_1\in D$ with $d_0<x<d_1$, using that $D$ is an [order-dense subset](../../../../../../../order-dense-subset.md). For $x\in D$, all its displayed values lie below $\varphi(x)$. If $y<\varphi(x)$, choose $e\in D$ with $y<e<\varphi(x)$; then $d=\varphi^{-1}(e)<x$. Thus the [supremum](../../../../../../../supremum.md) equals $\varphi(x)$.

The extension is strictly increasing. If $x<y$, choose $d,e\in D$ with $x<d<e<y$; then

$$
\widetilde\varphi(x)\leq\varphi(d)<\varphi(e)\leq\widetilde\varphi(y).
$$

Apply the same construction to $\varphi^{-1}$, obtaining $\psi$. For $d<x$, choose $e\in D$ with $d<e<x$; this gives $\varphi(d)<\widetilde\varphi(x)$. For $d>x$, a point of $D$ between $x$ and $d$ similarly gives $\varphi(d)>\widetilde\varphi(x)$. Hence

$$
\{e\in D:e<\widetilde\varphi(x)\}
=\{\varphi(d):d\in D, d<x\}.
$$

Taking inverse images and a [supremum](../../../../../../../supremum.md) shows $\psi(\widetilde\varphi(x))=x$. The symmetric argument gives $\widetilde\varphi(\psi(y))=y$, so the extension is an [order automorphism](../../../../../../../order-automorphism.md).

For uniqueness, any increasing extension $h$ has the same strict lower cut in $D$ at its value $h(x)$. Two distinct real numbers have different cuts in an [order-dense subset](../../../../../../../order-dense-subset.md), so $h(x)=\widetilde\varphi(x)$. **The extension exists and is unique.**

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 24](../../../../paper-24-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
