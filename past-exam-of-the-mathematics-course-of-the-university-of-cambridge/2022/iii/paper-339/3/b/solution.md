<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $P_f=\operatorname{prox}_f$ and $P_h=\operatorname{prox}_h$. Since $w_k=x_k+z_{k-1}$,

$$
y_k=P_h(w_k),
\qquad z_k=w_k-P_h(w_k),
$$

and therefore

$$
\boxed{w_{k+1}=T(w_k),
\qquad T=I-P_h+P_f(2P_h-I).}
$$

With reflected proximal maps $R_f=2P_f-I$ and $R_h=2P_h-I$,

$$
T=\frac12(I+R_fR_h).
$$

Firm nonexpansiveness of each proximal map is equivalent to nonexpansiveness of its reflection. Thus $R_fR_h$ is nonexpansive, and its average with the identity is firmly nonexpansive. This is the [Douglas–Rachford method](../../../../../../douglas-rachford-method.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
