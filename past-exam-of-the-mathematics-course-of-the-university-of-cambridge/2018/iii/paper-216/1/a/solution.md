<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $P$ be the [Markov kernel](../../../../../../markov-kernel.md) and $\mu$ its invariant [probability measure](../../../../../../probability-measure.md). Using the convention

$$
\|\nu-\mu\|_{\mathrm{TV}}=\sup_A|\nu(A)-\mu(A)|,
$$

[geometric ergodicity](../../../../../../geometric-ergodicity.md) means that there are $r\in(0,1)$ and a finite measurable state-dependent prefactor $M(x)$ such that

$$
\boxed{\|P^k(x,\cdot)-\mu\|_{\mathrm{TV}}\leq M(x)r^k\qquad(k\geq0).}
$$

Here [total variation distance](../../../../../../total-variation-distance.md) is used, and the rate $r$ does not depend on $x$. The prefactor need not be uniformly bounded; that stronger property is [uniform geometric ergodicity](../../../../../../uniform-geometric-ergodicity.md). For a deterministic starting state, this estimate must hold at that state. If the definition is made only $\mu$-almost everywhere, the subsequent assertions concern those starting states where the prefactor is finite. The [reversible Markov chain](../../../../../../reversible-markov-chain.md) assumption means $\mu(dx)P(x,dy)=\mu(dy)P(y,dx)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
