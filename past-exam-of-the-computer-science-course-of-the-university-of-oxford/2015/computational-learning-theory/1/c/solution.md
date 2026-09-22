<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose distinct points $x_1,\ldots,x_{d+2}$ of $S$. The $d+2$ [vectors](../../../../../vector.md) $(x_i,1)$ lie in the $(d+1)$-dimensional [vector space](../../../../../vector-space-split.md) $\mathbb R^{d+1}$, so they are [linearly dependent](../../../../../linear-dependence.md). Hence there are real numbers $\lambda_i$, not all zero, such that

$$
\sum_{i=1}^{d+2}\lambda_i x_i=0,\qquad\sum_{i=1}^{d+2}\lambda_i=0.
$$

The second equality forces both a positive and a negative coefficient. Put $I_+=\{i:\lambda_i>0\}$, $I_-=\{i:\lambda_i<0\}$, and

$$
L=\sum_{i\in I_+}\lambda_i=-\sum_{i\in I_-}\lambda_i>0.
$$

Rearranging the first equality gives

$$
\boxed{z=\sum_{i\in I_+}\frac{\lambda_i}{L}x_i
=\sum_{i\in I_-}\frac{-\lambda_i}{L}x_i.}
$$

Each side is a [convex combination](../../../../../convex-combination.md): the coefficients are positive and sum to one. Thus $z$ belongs to both [convex hulls](../../../../../convex-hull.md). Place the points with indices in $I_+$ in $A$, those with indices in $I_-$ in $B$, and assign every zero-coefficient point and every remaining point of $S$ to $A$. Then $A,B$ are nonempty, disjoint, and have union $S$. Adding points cannot shrink a [convex hull](../../../../../convex-hull.md), so

$$
\boxed{\operatorname{conv}(A)\cap\operatorname{conv}(B)\ne\varnothing.}
$$

This proves the [intersecting convex hull partition theorem](../../../../../radon-s-theorem.md), including when $S$ has more than $d+2$ points or is infinite: only the initial finite collection was needed.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Computational learning theory](../../../computational-learning-theory-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
