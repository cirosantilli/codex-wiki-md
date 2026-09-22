<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A feasible point lies in the [probability simplex](../../../../../../probability-simplex.md), so $r^Tx=\sum_i x_ir_i$ is a [convex combination](../../../../../../convex-combination.md) of the coordinates of $r$. Hence $r^Tx\le r_{\max}:=\max_i r_i$. Taking a coordinate vector $e_j$ with $r_j=r_{\max}$ attains equality. Therefore

$$
\boxed{v^*=\max_i r_i,\qquad x^*=e_j\ \text{for any }j\in\operatorname{argmax}_i r_i.}
$$

More generally, all optimal solutions are exactly the probability vectors supported on the maximizing indices: equality requires $x_i(r_{\max}-r_i)=0$ for every $i$. Thus ties give an entire optimal face, while a unique maximizing index gives a unique optimizer.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
