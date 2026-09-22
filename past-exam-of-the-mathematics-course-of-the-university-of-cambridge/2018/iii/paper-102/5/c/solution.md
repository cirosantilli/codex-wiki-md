<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We first prove the useful lemma that [dominant root-lattice highest weights have zero weight](../../../../../../dominant-root-lattice-highest-weights-have-zero-weight.md). Write $Q=\mathbb Z\Phi$ for the [root lattice](../../../../../../root-lattice.md), and let a [dominant integral weight](../../../../../../dominant-integral-weight.md) $\lambda\in Q$ be the [highest weight](../../../../../../highest-weight-of-a-representation.md) of a finite-dimensional irreducible representation.

First, $\lambda$ is a nonnegative integral combination of [simple roots](../../../../../../simple-root.md). Indeed, write $\lambda=\lambda_+-\lambda_-$, separating its positive and negative coefficients in the [root basis](../../../../../../fundamental-system-of-a-root-system.md). The two parts have disjoint supports, and distinct [simple roots](../../../../../../simple-root.md) have nonpositive [inner product](../../../../../../inner-product.md), so $(\lambda_+,\lambda_-)\leq0$. If $\lambda_-\ne0$, then

$$
(\lambda,\lambda_-)=(\lambda_+,\lambda_-)-(\lambda_-,\lambda_-)<0.
$$

On the other hand, dominance gives $(\lambda,\alpha_i)\geq0$ for each [simple root](../../../../../../simple-root.md), hence $(\lambda,\lambda_-)\geq0$. This contradiction proves $\lambda_-=0$.

Now suppose a nonzero weight $\mu=\sum_i m_i\alpha_i$ has all $m_i\in\mathbb Z_{\geq0}$. The identity

$$
0<(\mu,\mu)=\sum_i m_i(\mu,\alpha_i)
$$

shows that some $i$ satisfies $m_i>0$ and $\langle\mu,\alpha_i^\vee\rangle>0$. We use the standard [sl2 Lie algebra](../../../../../../sl2-lie-algebra.md) fact that its [lowering operator](../../../../../../lowering-operator.md) is injective on any positive $h$ eigenspace in a finite-dimensional representation. This follows from the [classification of finite-dimensional sl2 representations](../../../../../../classification-of-finite-dimensional-sl2-representations.md): in each irreducible $V(n)$, the only weight killed by the [lowering operator](../../../../../../lowering-operator.md) is the lowest weight $-n\leq0$.

Consequently a nonzero vector of weight $\mu$ lowers to a nonzero vector of weight $\mu-\alpha_i$. Its simple-root coefficients remain nonnegative and their sum decreases by one. Starting at $\lambda$, repeated lowering must therefore reach the zero weight. Notice that intermediate weights need not remain dominant; positivity of the chosen coroot pairing is enough at each step.

For a [minuscule representation](../../../../../../minuscule-representation.md), every weight belongs to $W\lambda$, so the zero weight just obtained lies in this orbit. Every [Weyl group](../../../../../../weyl-group.md) element is invertible, and $w\lambda=0$ forces $\lambda=0$. This proves that [minuscule weights in the root lattice are zero](../../../../../../minuscule-weights-in-the-root-lattice-are-zero.md). Under the assumption $X=Q$, every possible [highest weight](../../../../../../highest-weight-of-a-representation.md) lies in $Q$, hence

$$
\boxed{X=\mathbb Z\Phi\ \Longrightarrow\ \text{the only minuscule irreducible representation is }V(0),\text{ the trivial one}.}
$$

Here $V(0)$ is the one-dimensional [trivial Lie algebra representation](../../../../../../trivial-lie-algebra-representation.md), by the classification of finite-dimensional irreducible [highest-weight representations](../../../../../../highest-weight-representation.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
