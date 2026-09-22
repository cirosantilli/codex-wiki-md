<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $v_0$ be the highest vector of the [Verma module](../../../../../../verma-module.md) $M(n)$ and set $v_k=f^kv_0$. The [Poincaré-Birkhoff-Witt theorem](../../../../../../poincare-birkhoff-witt-theorem.md) implies that $(v_k)_{k\geq0}$ is a [basis](../../../../../../basis.md), so none of these vectors vanishes. The actions are

$$
f v_k=v_{k+1},\qquad h v_k=(n-2k)v_k,\qquad e v_k=k(n-k+1)v_{k-1}.
$$

The raising operator is a [locally nilpotent operator](../../../../../../locally-nilpotent-operator.md): on every vector, repeated application of $e$ eventually removes all its finitely many basis terms. Thus its [algebraic exponential of a locally nilpotent operator](../../../../../../algebraic-exponential-of-a-locally-nilpotent-operator.md) is defined, and $\exp(e)v_0=v_0$. But the middle factor in the proposed product would have to send this vector to

$$
\exp(-f)v_0=\sum_{k\geq0}\frac{(-1)^k}{k!}v_k,
$$

which has infinitely many nonzero, linearly independent basis coefficients. An element of the algebraic [Verma module](../../../../../../verma-module.md) is a finite linear combination of the $v_k$, so this expression is not in $M(n)$. In particular the lowering operator is not locally nilpotent.

Even for integral $n\geq0$, $f^{n+1}v_0$ is nonzero in the [Verma module](../../../../../../verma-module.md); it becomes zero only in its finite-dimensional irreducible quotient $L(n)$. Hence **$s$ is not defined as the displayed composition of endomorphisms of the algebraic Verma module**. Working in a completion would be a different problem and is not part of the module specified here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
