<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the first tableau the basis is $(x_2,s_5,x_1)$, giving

$$
x=(1/9,2/9,0),\qquad s=(0,2/3,0).
$$

The second basis is $(r_1,y_6,r_3)$, giving $y=(0,0,1/4)$ and $r=(3/4,0,1/4)$. This pair is not yet a [Nash equilibrium](../../../../../../nash-equilibrium.md): label $1$ is missing and label $4$ is duplicated.

Resolve the duplicate by bringing $y_4$ into the second tableau. Its column is $(3/4,1/4,9/4)^T$, so the [simplex ratio test](../../../../../../simplex-ratio-test.md) gives

$$
\min\left\{\frac{3/4}{3/4},\frac{1/4}{1/4},\frac{1/4}{9/4}\right\}=\frac19.
$$

Variable $r_3$ leaves, giving

$$
y=(1/9,0,2/9),\qquad r=(2/3,0,0).
$$

Now label $3$ is duplicated. Bring $x_3$ into the first tableau; its column is $(0,3,1)^T$. The positive-entry ratios are $(2/3)/3=2/9$ and $(1/9)/1=1/9$. Thus $x_1$ leaves, giving

$$
x=(0,2/9,1/9),\qquad s=(0,1/3,0).
$$

All labels are now present and $x_ir_i=y_js_j=0$. Each unnormalized strategy has total mass $1/3$, so the [Lemke-Howson algorithm](../../../../../../lemke-howson-algorithm.md) produces

$$
\boxed{x'=(0,2/3,1/3),\qquad y'=(1/3,0,2/3).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
