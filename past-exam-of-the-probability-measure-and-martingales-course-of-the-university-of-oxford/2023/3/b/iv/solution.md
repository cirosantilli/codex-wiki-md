<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $\mathcal G=T^{-1}(\mathcal F)=\{T^{-1}(A):A\in\mathcal F\}$. [Inverse images](../../../../../preimage.md) commute with [complements](../../../../../complement-of-a-set.md) and [countable unions](../../../../../countable-union.md), so this is a [sub-sigma-algebra](../../../../../sub-sigma-algebra.md) of $\mathcal F$. The [random variable](../../../../../random-variable-split.md) $X\circ T$ is $\mathcal G$-[measurable](../../../../../measurability.md).

The assumption $\mathbb P\circ T^{-1}=\mathbb P$ says that $T$ is a [measure-preserving transformation](../../../../../measure-preserving-transformation.md). Consequently $X\circ T$ has the same [probability distribution](../../../../../probability-distribution-split.md) as $X$ and is [integrable](../../../../../integrability.md). It also implies $\mathbb E[W\circ T]=\mathbb E[W]$ for every [integrable random variable](../../../../../integrable-random-variable.md) $W$, first for [indicator functions](../../../../../indicator-function.md), then for [simple functions](../../../../../simple-function.md), and then by positive and negative approximation.

To identify a [conditional expectation](../../../../../conditional-expectation.md), take any $A\in\mathcal F$. The assumed identity with the bounded [random variable](../../../../../random-variable-split.md) $Z=\mathbf1_A$ gives

$$
\begin{aligned}
\mathbb E[X\mathbf1_{T^{-1}(A)}]
&=\mathbb E[X(\mathbf1_A\circ T)]
=\mathbb E[X\mathbf1_A]\\
&=\mathbb E[(X\mathbf1_A)\circ T]
=\mathbb E[(X\circ T)\mathbf1_{T^{-1}(A)}].
\end{aligned}
$$

Every member of $\mathcal G$ has the displayed form $T^{-1}(A)$, so this verifies all defining [conditional expectation](../../../../../conditional-expectation.md) identities. Therefore

$$
\mathbb E[X\mid\mathcal G]=X\circ T\quad\text{almost surely}.
$$

Apply part (iii), since this [conditional expectation](../../../../../conditional-expectation.md) has the same [probability distribution](../../../../../probability-distribution-split.md) as $X$. We conclude

$$
\boxed{X=X\circ T\quad\mathbb P\text{-almost surely}.}
$$

This is [invariance from integral duality for a measure-preserving transformation](../../../../../invariance-from-integral-duality-for-a-measure-preserving-transformation.md); neither invertibility of $T$ nor a [second moment](../../../../../second-moment.md) of $X$ is required.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
