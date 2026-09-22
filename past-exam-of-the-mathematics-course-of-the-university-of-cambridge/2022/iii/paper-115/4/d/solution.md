<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $f=t\cos\theta+1$ and $g=\sin\theta$,

$$
\partial_tf-\partial_\theta g=\cos\theta-\cos\theta=0.
$$

The connection is therefore [flat](../../../../../../flat-principal-connection.md), so the [Frobenius theorem](../../../../../../frobenius-theorem.md) gives [horizontal sections](../../../../../../horizontal-section-of-a-principal-bundle.md) locally.

A global section has the form $z=h(\theta,t)$ and is horizontal exactly when

$$
\partial_\theta h=t\cos\theta+1,
\qquad
\partial_th=\sin\theta.
$$

The second equation gives $h=t\sin\theta+k(\theta)$, and the first then forces $k'(\theta)=1$. No such $k$ is periodic on $S^1$, so no global horizontal section exists. Equivalently, the horizontal lift of one positive circuit in the $\theta$ direction changes $z$ by

$$
\int_0^{2\pi}(t\cos\theta+1)\,d\theta=2\pi,
$$

which is nontrivial [holonomy](../../../../../../holonomy.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
