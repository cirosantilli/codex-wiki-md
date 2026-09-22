<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The two [Lasso](../../../../../../lasso.md) problems are

$$
\min_\beta\lVert Y-x\beta\rVert_2^2\quad\text{subject to }|\beta|\leq t
$$

and

$$
\min_{\beta_1,\beta_2}\lVert Y-x(\beta_1+\beta_2)\rVert_2^2
\quad\text{subject to }|\beta_1|+|\beta_2|\leq t.
$$

If $\widehat\beta$ solves the first problem, the complete solution set of the second is

$$
\boxed{\{(\beta_1,\beta_2):\beta_1+\beta_2=\widehat\beta,\ 
|\beta_1|+|\beta_2|\leq t\}}.
$$

Indeed, the feasible totals are exactly $[-t,t]$, the same as in the first problem.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
