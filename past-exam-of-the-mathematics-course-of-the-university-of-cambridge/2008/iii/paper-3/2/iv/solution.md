<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $v$ be a [highest-weight vector](../../../../../../highest-weight-vector.md) of weight $\lambda$. For a [simple root](../../../../../../simple-root.md) $\alpha_i$, choose its [sl2 subalgebra associated with a root](../../../../../../sl2-subalgebra-associated-with-a-root.md), with operators $E_i,F_i,H_i$ satisfying $[E_i,F_i]=H_i$, $[H_i,F_i]=-2F_i$, and $H_i=\alpha_i^\vee$. We have $E_iv=0$ and $H_iv=\lambda(H_i)v$.

Since $F_i$ decreases the weight by $\alpha_i$ and there are only finitely many [weights of a representation](../../../../../../weight-of-a-representation.md), let $n\geq0$ be maximal with $F_i^nv\ne0$. Induction using the two bracket relations gives the [sl2 highest-weight lowering formula](../../../../../../sl2-highest-weight-lowering-formula.md)

$$
E_iF_i^kv=k\bigl(\lambda(H_i)-k+1\bigr)F_i^{k-1}v.
$$

Applying this at $k=n+1$, the left side vanishes, and the nonzero vector $F_i^nv$ on the right forces $\lambda(H_i)=n$. This holds for every [simple root](../../../../../../simple-root.md), so

$$
\boxed{\langle\lambda,\alpha_i^\vee\rangle\in\mathbb Z_{\geq0}\text{ for all }i.}
$$

Thus the [highest weight](../../../../../../highest-weight-of-a-representation.md) is a [dominant integral weight](../../../../../../dominant-integral-weight.md), in particular an element of the [Closed dominant Weyl chamber](../../../../../../closed-dominant-weyl-chamber.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
