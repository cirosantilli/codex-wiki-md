<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an affine base, use the homogeneous equations furnished by the question, with fixed degrees $d_i$ in the projective coordinates. At a point $x$, the fiber $Y_x$ is the projective zero set of their specializations; a specialization may be zero, but is still assigned its original degree. Let

$$
I_x=(f_1(x,y),\ldots,f_r(x,y))\subseteq k[y_0,\ldots,y_n].
$$

Then $x\in\pi(Y)$ exactly when $Y_x$ is nonempty. Part (b) says this is equivalent to $I_x$ containing no power of the [irrelevant ideal of projective space](../../../../../../irrelevant-ideal-of-projective-space.md). In logical form, noncontainment must hold for every $N$, so

$$
\boxed{\pi(Y)=\bigcap_{N\ge0}\{x:I_x\not\supseteq\mathfrak m^N\}.}
$$

For schemes over an arbitrary field, replace $k$ in this fiber calculation by the residue field $\kappa(x)$ and use geometric fiber points. A point belongs to the scheme-theoretic topological image exactly when its fiber is nonempty, which is equivalent to nonemptiness after algebraic closure of that residue field.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
