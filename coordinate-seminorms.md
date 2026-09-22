# Coordinate seminorms

↑ **Parent:** [Seminorm](seminorm.md)

On $\mathbb R^2$, the [coordinate seminorms](coordinate-seminorms.md) $p_x$ and $p_y$ measure horizontal and vertical components separately. Their [kernels of seminorms](kernel-of-a-seminorm.md) are the vertical and horizontal axes. Neither is a [norm](norm.md), but together they form a [separating family of seminorms](separating-family-of-seminorms.md). A basic zero [neighbourhood](neighbourhood-mathematics.md) is

$$
\{p_x<a\}\cap\{p_y<b\}=(-a,a)\times(-b,b)\qquad(a,b>0).
$$

Each condition alone is an unbounded strip; their intersection is an open rectangle. For $a=b=1$, this is the unit [open ball](open-ball.md) of the [maximum norm](supremum-norm.md) $\|(x,y)\|_\infty=\max\{|x|,|y|\}$. For unequal tolerances it is the unit [open ball](open-ball.md) of the weighted [norm](norm.md) $\max\{|x|/a,|y|/b\}$. Thus the two coordinate measurements generate the usual [topology](topology-split.md) of the plane.

For a numerical check, take $a=1$, $b=1/2$: $(0.8,0.4)$ passes both tests, $(0.8,0.7)$ passes only the horizontal test, and $(1.2,0.4)$ passes only the vertical test. A direction missed by one [seminorm](seminorm.md) is detected by the other.

<a id="image-two-coordinate-seminorm-strips-intersect-in-a-basic-open-rectangle"></a>
![](seminorm-neighborhoods.png)

**[Figure 1](#image-two-coordinate-seminorm-strips-intersect-in-a-basic-open-rectangle). Two coordinate seminorm strips intersect in a basic open rectangle**.

## ↑ Ancestors (8)

1. [Seminorm](seminorm.md)
2. [Locally convex space](locally-convex-space.md)
3. [Topological vector space](topological-vector-space-split.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Coordinate seminorms](coordinate-seminorms.md)
