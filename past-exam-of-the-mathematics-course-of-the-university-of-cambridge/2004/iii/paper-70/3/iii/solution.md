<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the influence result and quadratic degree preservation to find each local limit piece, rather than assuming its smoothness. On $[x_i-h/2,x_i+h/2]$, only $y_{i-1},y_i,y_{i+1}$ matter. Extend these three values to a quadratic $P(x)=ax^2+bx+c$ across the uniform grid. Every refinement adds $3ah_r^2/16$, so the accumulated offset tends to

$$
\frac{3ah^2}{16}\sum_{r=0}^\infty4^{-r}=\frac{ah^2}{4}.
$$

By locality this gives the same limit as the original data on the chosen interval. Put $t=(x-x_i)/h$ and $D_i=y_{i-1}-2y_i+y_{i+1}$. The limit piece is consequently

$$
s(x_i+th)=y_i+\frac{D_i}{8}+\frac{y_{i+1}-y_{i-1}}2t+\frac{D_i}{2}t^2,\qquad-1/2\leq t\leq1/2.
$$

At the right edge center it has

$$
s(x_i+h/2)=\frac{y_i+y_{i+1}}2,\qquad s'(x_i+h/2)=\frac{y_{i+1}-y_i}{h}.
$$

The next piece gives the same value and derivative at its left endpoint. The second derivatives on the two sides are instead $D_i/h^2$ and $D_{i+1}/h^2$, which generally differ. Hence

$$
\boxed{s\in C^1\text{ at each original edge center, but generally }s\notin C^2.}
$$

There is one continuous derivative in addition to the continuous curve itself. Special data such as a globally quadratic sequence can make higher derivatives match.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
