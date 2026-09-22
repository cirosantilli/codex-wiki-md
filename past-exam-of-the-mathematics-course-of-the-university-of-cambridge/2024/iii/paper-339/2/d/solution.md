<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take $a=\mathbf1$ and $b=k$, so

$$
C=\left\{v\in\mathbb R^n:
0\leq v_i\leq1,\ \sum_{i=1}^nv_i=k\right\}
$$

is the [capped simplex](../../../../../../capped-simplex.md). A linear objective over this [convex polytope](../../../../../../convex-polytope.md) attains its maximum at a zero-one extreme point. Choosing the $k$ coordinates at which $x_i$ is largest gives

$$
\max_{v\in C}x^Tv=x_{[1]}+\cdots+x_{[k]}=h(x).
$$

Equivalently, an exchange of weight from a smaller component to a larger one never decreases the objective. Thus the [sum of the largest components](../../../../../../sum-of-the-largest-components.md) is the [support function](../../../../../../support-function.md) $\sigma_C$.

Part c now gives

$$
\operatorname{prox}_{th}(y)=y-tP_C(y/t).
$$

By the [projection onto a box-constrained hyperplane](../../../../../../projection-onto-a-box-constrained-hyperplane.md), $v=P_C(y/t)$ has

$$
v_i=\min\{1,\max\{0,y_i/t-\nu\}\},
\qquad
\sum_i v_i=k.
$$

**Consequently the proximal operator is evaluated by solving this one-dimensional equation for $\nu$, then substituting the resulting projection.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
