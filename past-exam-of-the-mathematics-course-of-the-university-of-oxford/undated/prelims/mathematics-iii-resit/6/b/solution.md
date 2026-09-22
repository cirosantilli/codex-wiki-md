<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each nonnegative integer $z$, the [events](../../../../../../event.md) $\{X=z-y,Y=y\}$, $0\le y\le z$, are pairwise disjoint and their union is $\{X+Y=z\}$. By [countable additivity](../../../../../../countable-additivity.md) and then [independence](../../../../../../independent-random-variables.md),

$$
\begin{aligned}
p_Z(z)&=\sum_{y=0}^z\mathbb P(X=z-y,Y=y)\\
&=\boxed{\sum_{y=0}^zp_Y(y)p_X(z-y).}
\end{aligned}
$$

This is the [discrete convolution](../../../../../../discrete-convolution.md) of the two [probability mass functions](../../../../../../probability-mass-function.md). If the convention for natural numbers excludes zero, set both [probability mass functions](../../../../../../probability-mass-function.md) equal to zero there; the formula remains valid. Also $p_Z(z)=0$ for negative $z$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Mathematics III resit](../../../mathematics-iii-resit-split.md)
4. [Prelims](../../../split.md)
5. [Undated](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
